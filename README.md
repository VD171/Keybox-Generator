# Keybox Generator
This script uses the private key of an existing keybox file for generating a new certificate and appending it into a "new" keybox file.  
  
### This is for educational purpose.  
### Never buy a four-certificates keybox.  
  
## Usage  
### Download
```sh
curl -o Keybox-Generator.py https://raw.githubusercontent.com/VD171/Keybox-Generator/refs/heads/main/Keybox-Generator.py
```
### Run
```sh
python Keybox-Generator.py --file keybox.xml --days 365 --title "New certificate generated by @VD_Priv8" --serial_ca 171 --serial_subject VDPriv8 --out keybox.new.xml
```
#### For a valid keychain, use
```sh
--title TEE --serial_ca random --serial_subject random
```
  
## Arguments
All arguments are optional. If not present, default is used.
| Argument             | Default                        | Description                                                                 |
|----------------------|--------------------------------|-----------------------------------------------------------------------------|
| `--file`             | `keybox.xml`                   | Keybox file path.                                                          |
| `--days`             | `365`                          | How many days for expiring the new certificate.                           |
| `--title`            | `New certificate generated by @VD_Priv8` | Title for the new certificate. Use `TEE` for a valid title.         |
| `--serial_ca`        | `171`                          | Set the unique Serial for the new certificate (hex format). Use `random` for a valid Serial. |
| `--serial_subject`   | `VDPriv8`                        | Set `serialNumber` in Subject for the new certificate. Use `random` for a valid serialNumber. |
| `--out`              | `keybox.new.xml`               | Output path for the new Keybox file.                                       |

  
## Keybox Checker  
Check your keyboxes using only the best keybox checker:  
https://t.me/KeyBox_Checker_by_VD_Priv8_bot  
  
## Telegram
https://t.me/VD_Priv8  
https://t.me/RootDetected  
https://t.me/BlankAssistance  
  
## License  
This project is licensed under the **GNU Affero General Public License v3.0**.  
For more details, see the [LICENSE](LICENSE) file.  

