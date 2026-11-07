# URL Investigation

## 1. Investigation Overview

**Investigation Type:** Phishing URL Analysis
**Target URL:** http://login-micros0ft-support.example/verify
**Classification:** Simulated Phishing URL
**Purpose:** SOC Analyst L1 Portfolio Project

## 2. Initial URL Inspection

The URL was extracted from a simulated phishing email impersonating Microsoft Security.

Initial observations:

* The URL uses HTTP instead of HTTPS.
* The domain contains a brand impersonation attempt.
* The word "Microsoft" is misspelled as "micros0ft", replacing the letter "o" with the number zero.
* The URL contains a `/verify` path, suggesting an account verification action.

## 3. Domain Examination

The domain is:

`login-micros0ft-support.example`

The `.example` top-level domain is reserved for documentation and testing.

Therefore, this URL is simulated and is not evidence of a live phishing website.

## 4. Security Indicators

| Indicator              | Observation                  |
| ---------------------- | ---------------------------- |
| Brand impersonation    | Microsoft                    |
| Character substitution | Letter o replaced with 0     |
| Protocol               | HTTP                         |
| URL path               | /verify                      |
| Domain extension       | .example                     |
| Classification         | Simulated phishing indicator |

## 5. Security Assessment

The URL demonstrates characteristics commonly associated with phishing attempts:

1. Brand impersonation.
2. Deceptive domain naming.
3. Account verification language.
4. Potential credential-harvesting intent.

However, these characteristics alone do not establish that a website is malicious.

The reserved `.example` domain means this sample cannot be treated as evidence of an operational phishing website.

## 6. Analyst Conclusion

The URL was classified as a simulated phishing indicator based on its structure and context within the sample email.

No claim of live malicious activity, successful credential theft, or confirmed malware delivery is made.

**Final Classification:** Simulated Phishing URL — Educational Investigation.
