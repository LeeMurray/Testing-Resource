# EMAIL TESTING

## VALID EMAIL

| Email Address | Reason |
| --- | --- |
| email@domain.com | Valid Email |
| firstname.lastname@domain.com | Email contains dot in the address field |
| email@subdomain.domain.com | Email contains dot with subdomain |
| firstname+lastname@domain.com | Plus sign is considered valid character |
| email@123.123.123.123 | Domain is valid IP address |
| email@[123.123.123.123] | Square bracket around IP is considered valid |
| 1234567890@domain.com | Digets in domain name is valid |
| email@domain-one.com | Dash in domain name is valid |
| email@domain.name | .name is valid Top Level Domain name |
| email@domain.co.jp | Dot in Top Level Domain name also considered valid (use co.jp as example here) |
| firstname-lastname@domain.com | Dash in address field is valid |

---

## INVALID EMAIL

| Email Address | Reason |
| --- | --- |
| plainaddress | Missing the @ sign and domain |
| @%^%#$@#$@#.com | Garbage |
| @domain.com | Missing username |
| Joe Smith <email@domain.com> | Encoded html within email is invalid |
| email.domain.com | Missing @ |
| email@domain@domain.com | Two @ signs |
| .email@domain.com | Leading dot in address is not allowed |
| email.@domain.com | Trailing dot in address is not allowed |
| email..email@domain.com | Multipul dots |
| À@domain.com | Unicode char as address |
| email@domain.com (Joe Smith) | Text following email is no allowed |
| email@domain | Missing top level domain (.com/.net/.org/etc) |
| email@-domain.com | Leading dash in front of domain is invalid |
| email@domain.web | .web is not a valid top level domain |
| email@11.22.33.44444 | Invalid IP format |
| email@domain..com | Multipul dot in the domain portion is invalid |

---