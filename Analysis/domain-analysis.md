# Domain Investigation

## 1. Investigation Overview

**Investigation Type:** Domain Reputation and Infrastructure Analysis
**Target Domain:** login-micros0ft-support.example
**Investigation Context:** Simulated phishing email
**Role:** SOC Analyst L1

## 2. Domain Characteristics

The domain was extracted from the suspicious URL found in the sample phishing email.

Key observations:

* The domain imitates Microsoft's brand identity.
* The letter "o" is replaced with the number "0".
* The domain uses a `.example` extension.
* The naming structure attempts to create the appearance of a legitimate account support service.

## 3. Domain Registration and Reputation

The `.example` top-level domain is reserved for documentation and testing.

Consequently:

* Public domain registration information is not applicable.
* Live DNS resolution is not expected.
* Domain reputation cannot establish whether this simulated domain is malicious.
* No live infrastructure attribution can be made.

## 4. Infrastructure Investigation

During the broader investigation, VirusTotal was used to examine URL and domain-related indicators.

The investigation also included reviewing:

* IP address information.
* Autonomous System Numbers (ASN).
* Network ownership.
* Security vendor detection results.
* Domain and URL reputation.

One observed infrastructure indicator was:

| Attribute    | Observation    |
| ------------ | -------------- |
| Network      | 2607:f8b0::/32 |
| ASN          | AS15169        |
| Organization | Google LLC     |
| RIR          | ARIN           |
| Country      | United States  |

**Important:** This is a separately observed network indicator from the investigation. It must not be attributed to the simulated `.example` domain without verified DNS or infrastructure correlation.

Google-associated infrastructure and clean vendor detections do not independently establish that an investigated URL is safe.

## 5. Security Assessment

The domain naming pattern demonstrates characteristics associated with brand impersonation.

However, domain appearance alone is insufficient to establish malicious activity.

The reserved `.example` extension confirms that the email sample is simulated rather than a live phishing domain.

## 6. Analyst Conclusion

The investigation identified suspicious domain-naming characteristics and documented relevant infrastructure observations.

No confirmed malicious infrastructure, domain registration, or live phishing activity is claimed.

**Final Classification:** Simulated Phishing Domain — Educational Investigation.
