---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onclusive.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=50; rua=mailto:airadmin@airpr.com
  dnssec: false
  domain: airpr.com
  note: DMARC is still enforced at only 50% sampling (pct=50) and reports still go to an @airpr.com mailbox years after the Onclusive acquisition.
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.google.com include:_spf.salesforce.com include:mktomail.com include:sendgrid.net ~all
hosts:
- cert_expires: Oct  1 21:56:45 2026 GMT
  host: onclusive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 15:02:40 2026 GMT
  host: airpr.com
  hsts: false
  https: true
  note: Still live and separately certificated, but 301s to onclusive.com. DNS is an ALIAS to airpr.com.herokudns.com — the original AirPR Heroku estate.
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: developer.onclusive.com
  hsts: false
  https: true
  note: CloudFront in front of an S3 origin (AWS API Gateway Developer Portal)
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: crawler-api-auth.onclusive.com
  hsts: false
  https: true
  note: Amazon Cognito hosted UI for user pool us-east-1_F0XmSWr9T
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airpr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirPR, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AirPR
provider_slug: airpr
slug: airpr-domain-security
source_filename: airpr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + the developer-portal and auth hosts\nnote: >-\n  Extends the mechanical probe (probe-domain-security.py, which resolves only\n  the apis.yml Website host) with the three further hosts contract discovery\n  turned up: the legacy airpr.com origin, the AWS-hosted developer portal, and\n  the Cognito hosted-UI domain that fronts it. No host in this estate sets HSTS,\n  and neither registrable domain is DNSSEC-signed or publishes a CAA record.\nhosts:\n- host: onclusive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 21:56:45 2026 GMT\n  hsts: false\n- host: airpr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:02:40 2026 GMT\n  hsts: false\n  note: >-\n    Still live and separately certificated, but 301s to onclusive.com. DNS is an\n    ALIAS to airpr.com.herokudns.com — the original AirPR Heroku estate.\n- host: developer.onclusive.com\n  https:\
  \ true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\n  note: CloudFront in front of an S3 origin (AWS API Gateway Developer Portal)\n- host: crawler-api-auth.onclusive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\n  note: Amazon Cognito hosted UI for user pool us-east-1_F0XmSWr9T\ndomains:\n- domain: onclusive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: airpr.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: >-\n    v=spf1 include:spf.protection.outlook.com include:_spf.google.com\n    include:_spf.salesforce.com include:mktomail.com include:sendgrid.net ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; pct=50; rua=mailto:airadmin@airpr.com'\n  note: >-\n    DMARC is still enforced at only 50% sampling (pct=50) and reports still go\n    to an @airpr.com mailbox years after the Onclusive acquisition.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airpr/refs/heads/main/security/airpr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Public Relations
- Media Intelligence
- Media Monitoring
- Analytics
- Communications
- Marketing
- PR Measurement
- Onclusive
---
