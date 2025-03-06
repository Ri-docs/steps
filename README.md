
## 1. Create a new form.
![alt text](image.png)

## 2. Add a new form item by placing mouse under description
![alt text](image-1.png)

## 3. Use an input field
![alt text](image-2.png)

## 4. Give it a name and ID
![alt text](image-3.png)

## 5. While in edit mode, Mouse over the line connecting to the next Action to add a new Action
![alt text](image-4.png)

## 6 In the Visibility Per Step tab Set the Start Action field to `hidden`

![alt text](image-8.png)
## 7. You will need to use the Connect (Advanced Action)
![alt text](image-5.png)

## 8. Fill out the action with these settings
![alt text](image-6.png)
- The key value pairs I used are:
```sh
expires='%{request.customExpirationPeriod}'
defaultExpires={"years": 1}
```
> Note: The defaultExpires field should match the expiration you put on the entitlement when you created it. You can place more or less time like so:
```sh
defaultExpires={"years": 1, "months: 10", "weeks": 2, "days": 7, "hours": 10, "minutes": 30}
```

## 9. You will need another Action (Update Form) added after the Connect Action
![alt text](image-7.png)

## 10. Upload the action set into connect
![](image-9.png)

## 11. If you want to change how the date is formatted, you can adjust that in the Action Set
![alt text](image-10.png)

> It uses Java 8 formatting codes.

## 12. Test a user and ensure you can see the Expiration populate in the approval step.

