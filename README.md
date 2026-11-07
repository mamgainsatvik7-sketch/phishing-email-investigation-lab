# Phishing Email Investigation Lab

### SOC Analyst L1 | Cybersecurity Portfolio Project

## Project Overview

This project demonstrates a structured phishing email investigation workflow from the perspective of a Level 1 Security Operations Center (SOC) Analyst.

The investigation focuses on identifying phishing indicators, examining email authentication results, analyzing suspicious URLs, investigating domain characteristics and documenting findings in an incident report.

The project combines simulated phishing evidence with practical security investigation techniques.

## Objectives

* Identify common phishing indicators.
* Investigate suspicious sender addresses and domains.
* Understand SPF, DKIM and DMARC authentication.
* Analyze suspicious URLs using VirusTotal.
* Examine IP addresses, ASN information and network ownership.
* Document investigation findings.
* Develop an L1 SOC phishing investigation playbook.

## Tools Used

| Tool                 | Purpose                                   |
| -------------------- | ----------------------------------------- |
| VirusTotal           | URL and domain reputation analysis        |
| Google Admin Toolbox | Email header analysis                     |
| GitHub               | Investigation documentation and portfolio |
| Web Browser          | Manual security investigation             |

## Investigation Workflow

The investigation followed these stages:

1. **Email Analysis:** Examined sender identity, suspicious wording and phishing indicators.
2. **Email Authentication:** Reviewed SPF, DKIM and DMARC results.
3. **URL Investigation:** Examined suspicious URL characteristics and reputation.
4. **Domain Investigation:** Reviewed domain characteristics and available infrastructure information.
5. **Threat Assessment:** Evaluated findings and documented investigation limitations.
6. **Incident Reporting:** Prepared a structured incident investigation report.
7. **Playbook Development:** Documented a repeatable phishing investigation procedure.

## Repository Structure

```text
phishing-email-investigation-lab/
│
├── README.md
│
├── Evidence/
│   └── sample-phishing-email.txt
│
├── Analysis/
│   ├── url-analysis.md
│   └── domain-analysis.md
│
├── Reports/
│   └── phishing-incident-report.md
│
├── Screenshots/
│   └── README.md
│
└── Playbooks/
    └── phishing-investigation-playbook.md
```

## Key Investigation Findings

The investigation documented the following phishing characteristics:

* Brand impersonation.
* Suspicious sender identity.
* Character substitution in domain naming.
* Urgency-based social engineering.
* SPF authentication failure in the examined header-analysis output.
* Suspicious URL characteristics.
* IP address and ASN infrastructure observations.

### Infrastructure Observation

One separately observed network indicator:

| Attribute    | Value          |
| ------------ | -------------- |
| Network      | 2607:f8b0::/32 |
| ASN          | AS15169        |
| Organization | Google LLC     |
| Country      | United States  |

This infrastructure observation was documented separately and was not attributed to the simulated phishing domain without verified correlation.

## Incident Assessment

**Classification:** Simulated Phishing Investigation

The investigation demonstrated common phishing characteristics and practical investigation techniques.

No confirmed credential theft, account compromise, malware execution or live malicious infrastructure was established.

## Analyst Skills Demonstrated

* Phishing email investigation.
* Email header analysis.
* SPF, DKIM and DMARC fundamentals.
* URL investigation.
* Domain analysis.
* IP and ASN examination.
* Threat intelligence fundamentals.
* Incident documentation.
* SOC investigation workflow development.

## Limitations

This is an educational portfolio project.

The phishing email uses a reserved `.example` domain for simulation. It does not represent an operational phishing website.

Infrastructure observations are documented separately and should not be interpreted as proof of malicious activity.

## Project Status

| Component               | Status    |
| ----------------------- | --------- |
| Phishing Email Evidence | Completed |
| URL Analysis            | Completed |
| Domain Analysis         | Completed |
| Incident Report         | Completed |
| Investigation Playbook  | Completed |
| Screenshots             | Pending   |
| Documentation           | Completed |

## Author

**Satvik Mamgain**

Aspiring SOC Analyst | Cybersecurity Enthusiast

GitHub: [@mamgainsatvik7-sketch](https://github.com/mamgainsatvik7-sketch)
