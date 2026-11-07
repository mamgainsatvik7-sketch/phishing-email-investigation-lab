# Phishing Incident Investigation Report

## 1. Incident Overview

| Field                | Details                               |
| -------------------- | ------------------------------------- |
| Incident Type        | Suspected Phishing Email              |
| Severity             | Medium — Educational Assessment       |
| Investigation Status | Completed                             |
| Analyst Role         | SOC Analyst L1                        |
| Investigation Method | Email Header, URL and Domain Analysis |
| Environment          | Simulated Investigation Lab           |

## 2. Executive Summary

A suspicious email impersonating Microsoft Security was investigated for potential phishing activity.

The email contained urgency-based language, a suspicious sender domain and a URL designed to resemble a legitimate Microsoft account verification service.

The investigation focused on identifying indicators of phishing, examining email authentication results and evaluating the associated URL and domain characteristics.

The sample was simulated for educational purposes. No real victim, compromised account or confirmed malicious infrastructure was identified.

## 3. Indicators of Suspicious Activity

The following indicators were identified:

1. Sender identity inconsistent with legitimate Microsoft branding.
2. Character substitution in the domain name.
3. Suspicious account verification URL.
4. Urgency-based language intended to encourage immediate action.
5. HTTP protocol rather than HTTPS.

## 4. Email Authentication Analysis

Email authentication mechanisms were examined:

* SPF (Sender Policy Framework)
* DKIM (DomainKeys Identified Mail)
* DMARC (Domain-based Message Authentication, Reporting and Conformance)

The examined header-analysis output showed an SPF failure.

This is a potential authentication concern but does not independently prove phishing.

## 5. URL and Domain Investigation

The URL was examined for:

* Domain impersonation.
* Suspicious URL structure.
* Brand impersonation techniques.
* Reputation and security vendor detections.
* Associated network infrastructure.

The sample used a reserved `.example` domain.

Therefore, live domain registration, DNS resolution and operational infrastructure could not be established for the sample URL.

## 6. Tools Used

| Tool                               | Purpose                                 |
| ---------------------------------- | --------------------------------------- |
| Google Admin Toolbox Messageheader | Email header analysis                   |
| VirusTotal                         | URL and domain reputation investigation |
| Web browser                        | Manual indicator inspection             |
| GitHub                             | Investigation documentation             |

## 7. Findings and Limitations

The investigation identified multiple phishing-like characteristics.

However, the available evidence does not establish:

* Successful credential theft.
* Actual account compromise.
* Successful malware delivery.
* Live malicious infrastructure.
* Confirmed financial or operational impact.

An observed Google-associated network range (AS15169) was documented separately. No verified relationship between that infrastructure and the simulated domain was established.

## 8. Recommended Response

If this were a real organizational incident, the recommended response would be:

1. Quarantine the suspicious email.
2. Identify other recipients of the same message.
3. Block confirmed malicious sender addresses and URLs.
4. Review email gateway and authentication logs.
5. Investigate whether any recipient clicked the link.
6. Check for suspicious authentication activity.
7. Reset credentials and revoke active sessions if compromise is confirmed.
8. Escalate the incident according to organizational procedures.

## 9. Final Assessment

**Classification:** Suspected Phishing — Simulated Investigation.

The investigation demonstrated the identification of suspicious email characteristics, email authentication analysis, URL inspection and domain investigation.

The findings are consistent with common phishing techniques, but no live malicious activity or successful compromise was established.

**Investigation Status:** Completed — Educational Lab.
