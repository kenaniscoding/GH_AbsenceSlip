# LSGH Absence Slip

## Features
- Automatic Email to Parent/Student and Teacher
- Admin changable Grade Level, Subjects, and Teachers
- Admin login to change status of absence slip
  
## Tech Stack
- **Frontend:** JavaScript (Ajax), CSS, HTML
- **Backend:** MySQL and PHP (XAMPP)


## Requirements
- To run this project, you will need to have [XAMPP](https://www.apachefriends.org/download.html) installed 
- Gmail account not older than 2024
- Windows 10/11 is recommended for the email to work
- To secure the phpmyadmin, go to C:\xampp\phpMyAdmin\config.inc.php and edit to cookie [video steps](https://youtu.be/LltCLFxQ2Yk?si=AbBG43zsRuVZp2nM)
```bash
    $cfg['Servers'][$i]['auth_type'] = 'cookie';
```


## Troubleshooting

To configure the email, go to C:xampp\php and open the `Php.ini` then go the `[mail function]` and edit these

```bash
  [mail function]
  For Win32 only.
  http://php.net/smtp
  SMTP=smtp.gmail.com
  http://php.net/smtp-port
  smtp_port=587
  sendmail_from = youremailaddress@gmail.com
  sendmail_path = "\"C:\xampp\sendmail\sendmail.exe\" -t"
```

If you don't have your google app password for your email address then go here

[App Password](https://myaccount.google.com/apppasswords)
[Documentation](https://support.google.com/accounts/answer/185833?hl=en#:~:text=Create%20%26%20use%20App%20Passwords)


Next go to C:xampp\sendmail and open the `sendmail.ini` then go the `[sendmail]` and edit these

```bash
  smtp_server=smtp.gmail.com
  smtp_port=587
  error_logfile=error.log
  debug_logfile=debug.log
  auth_username=youremailaddress@gmail.com
  auth_password=google_app_password
  force_sender=youremailaddress@gmail.com (OPTIONAL)
```

### Helpful Guides for the Email

[Email Feature Steps](https://www.codingnepalweb.com/configure-xampp-to-send-mail-from-localhost/)

[YouTube Video on Email Feature](https://youtu.be/KA2UB3pxEtg?si=2_AK-gLmpzjFWim0)

## Preview



