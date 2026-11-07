# SOC L1 Phishing Investigation Playbook

## 1. Purpose

This playbook provides a structured procedure for investigating suspected phishing emails in a Security Operations Center (SOC).

It is designed for entry-level SOC analysts handling phishing alerts.

## 2. Investigation Workflow

### Step 1: Review the Alert

* Identify the alert source.
* Record the alert timestamp.
* Identify the recipient.
* Review the email subject.
* Determine whether the email contains suspicious attachments or links.

### Step 2: Examine the Sender

Inspect:

* Sender email address.
* Sender display name.
* Reply-To address.
* Return-Path.
* Sender domain.

Look for:

* Domain impersonation.
* Misspelled domains.
* Unusual sender addresses.
* Mismatched display names.

### Step 3: Analyze Email Headers

Use an email header analysis tool.

Check:

* SPF authentication.
* DKIM authentication.
* DMARC authentication.
* Received headers.
* Sending IP address.
* Sender infrastructure.

Important:

An SPF, DKIM or DMARC failure is an indicator requiring investigation, not automatic proof of phishing.

### Step 4: Investigate URLs

Extract URLs without opening them directly.

Use reputation-analysis tools such as VirusTotal.

Check:

1. URL reputation.
2. Domain reputation.
3. Security vendor detections.
4. Redirect behavior.
5. Final destination.
6. URL creation and registration information, where available.

Never visit a suspicious URL from a normal workstation.

### Step 5: Investigate Attachments

If attachments are present:

* Identify the file type.
* Calculate the file hash.
* Check the hash using VirusTotal.
* Review available security vendor detections.
* Escalate suspicious files for sandbox analysis.

Do not execute suspicious attachments on a production workstation.

### Step 6: Check User Interaction

Determine whether the recipient:

* Opened the email.
* Clicked the URL.
* Downloaded an attachment.
* Entered credentials.
* Approved an unexpected MFA request.

Correlate findings with available email gateway, endpoint and identity logs.

### Step 7: Determine Severity

Suggested assessment:

| Severity | Example                                                                    |
| -------- | -------------------------------------------------------------------------- |
| Critical | Confirmed account compromise with ongoing malicious activity               |
| High     | Confirmed credential theft or malware execution                            |
| Medium   | Suspicious email delivered or clicked, with no confirmed compromise        |
| Low      | Suspicious characteristics but insufficient evidence of malicious activity |

Follow organizational severity definitions and escalation procedures.

### Step 8: Containment and Escalation

Depending on organizational authorization:

* Quarantine malicious emails.
* Block confirmed malicious URLs and domains.
* Identify other affected recipients.
* Request credential resets where compromise is confirmed.
* Revoke active sessions if necessary.
* Escalate confirmed compromise to the appropriate SOC team.

Do not independently perform actions outside your assigned permissions.

### Step 9: Document Findings

Record:

* Alert ID.
* Timestamp.
* Sender address.
* Recipient.
* Email subject.
* Suspicious URLs.
* Attachment hashes.
* Authentication results.
* VirusTotal findings.
* User interaction.
* Investigation conclusion.
* Containment actions.
* Escalation status.

## 3. Investigation Tools

| Tool                 | Usage                                     |
| -------------------- | ----------------------------------------- |
| VirusTotal           | URL, domain and file reputation           |
| Google Admin Toolbox | Email header analysis                     |
| Windows Event Viewer | Authentication and endpoint investigation |
| SIEM (Splunk)        | Log correlation and alert investigation   |
| GitHub               | Investigation documentation               |

## 4. Analyst Decision

After collecting evidence, classify the alert as:

* Confirmed Phishing
* Likely Phishing
* Benign / False Positive
* Inconclusive — Requires Escalation

Never classify an email as malicious based on a single indicator.

## 5. Final Objective

The objective of an L1 SOC analyst is to identify suspicious activity, collect relevant evidence, assess potential impact, perform authorized containment actions and escalate incidents when required.

**Playbook Status:** Completed — Educational SOC Portfolio.
