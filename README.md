# Message Box

# Description
A module to show message boxes in Windows-based Python applications.

# Usage
## Parameters
### title: str
- The title shown on message box.
- Default is 'My title'.
### text: str
- The text shown on message box.
- Default is 'My text'.
### button: str
- The button(s) shown on message box.
- Options include: 'OK' (default), 'OKCANCEL', 'ABORTRETRYIGNORE', 'YESNOCANCEL', 'YESNO', 'RETRYCANCEL',  'CANCELTRYCONTINUE', 'OKHELP'
### icon: str
- The icon shown on message box.
- Options include: 'NOICON', 'ICONSTOP', 'ICONERROR', 'ICONHAND', 'ICONQUESTION', 'ICONEXCLAMATION', 'ICONWARNING', 'ICONINFORMATION' (default), 'ICONASTERISK'

## Return
### value: str
- The button the user clicked on message box.
- Values include: 'OK', 'CANCEL', 'ABORT',  'RETRY', 'IGNORE',  'YES', 'NO', 'TRYAGAIN', 'CONTINUE'

## Examples
### To show an information message box with **OK** and **Cancel** buttons:
```python
import mbox

mbox.show(title='My Message Box', text='My message', button='OKCANCEL')
```
![Info msg ok-cancel](images/Info%20msg%20ok-cancel.png)

### To show an error message box with an **OK** button:
```python
import mbox

mbox.show(title='My Message Box', text='My message', icon='ICONERROR')
```
![Error msg ok](images/Error%20msg%20ok.png)

### Some other possible options include:
#### No icon with **Yes** and **No** buttons:
![No icon msg yes-no](images/No%20icon%20msg%20yes-no.png)

#### Warning icon with **OK** and **Help** buttons:
![Warning msg ok-help](images/Warning%20msg%20ok-help.png)

#### Question icon with **Abort**, **Retry**, and **Ignore** buttons:
![Question msg abort-retry-ignore](images/Question%20msg%20abort-retry-ignore.png)

# Dependencies
- Python 3.x
- Windows

# License
Licensed under the [MIT License](LICENSE)
