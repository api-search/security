---
description: ''
domains:
- caa: []
  caa_note: No CAA record — any public CA may issue for this domain.
  dmarc: false
  dmarc_note: No _dmarc.sensestreet.com TXT record. SPF is published with a -all hard fail but without DMARC there is no reporting and no policy applied to the header From — a gap worth closing for a vendor whose customers are banks.
  dnssec: false
  domain: sensestreet.com
  mx: sensestreet-com.mail.protection.outlook.com
  spf: true
  spf_policy: hard-fail
  spf_record: v=spf1 include:spf.protection.outlook.com ip4:20.90.220.112 -all
hosts:
- cert_expires: Oct  5 13:15:53 2026 GMT
  host: sensestreet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:38:40 2026 GMT
  cert_issued: Jul  7 21:38:41 2026 GMT
  cert_subject: CN=www.sensestreet.com
  cert_valid: true
  host: www.sensestreet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
- cert_expires: Oct  5 15:08:55 2026 GMT
  cert_issued: Jul  7 15:08:56 2026 GMT
  cert_subject: CN=docs.sensestreet.com
  cert_valid: true
  host: docs.sensestreet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
- cert_expires: May  3 08:31:23 2026 GMT
  cert_issued: Feb  2 08:31:24 2026 GMT
  cert_issuer: C=US, O=Let's Encrypt, CN=R13
  cert_subject: CN=sensestreet.com
  cert_valid: false
  finding: expired-certificate
  finding_detail: 'The customer-facing Sense Street portal — the host that also serves the live /api/v1 surface — presents a Let''s Encrypt certificate that expired on 2026-05-03, more than three months before this probe. curl refuses the connection with exit 60 (certificate verify failed) and every browser will interstitial. This is the single most material security finding on the domain, and it is trivially fixable: the same wildcard was renewed on the Framer-hosted marketing hosts but not here.'
  host: portal.sensestreet.com
  hsts: false
  hsts_note: No Strict-Transport-Security header on the portal, unlike the marketing and docs hosts which both set max-age=31536000.
  https: true
  sans_note: 'The SAN list is itself a public disclosure of the deployment topology: a per-tenant production API pattern (*.api.sensestreet.com), a matching test environment (*.api.test.sensestreet.com), a separate auth surface (*.auth.sensestreet.com), and both AWS and GCP delivery targets (*.aws / *.gcp.sensestreet.com).'
  wildcard_sans:
  - '*.api.sensestreet.com'
  - '*.api.test.sensestreet.com'
  - '*.auth.sensestreet.com'
  - '*.aws.sensestreet.com'
  - '*.ds.sensestreet.com'
  - '*.gcp.sensestreet.com'
  - '*.sensestreet.co.uk'
  - '*.sensestreet.com'
  - sensestreet.co.uk
  - sensestreet.com
kind: domain-security
layout: security
method: probed
name: Sense Street Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sense Street, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sense Street
provider_slug: sense-street
slug: sense-street-domain-security
source_filename: sense-street-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every reachable Sense Street host\nhosts:\n- host: sensestreet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 13:15:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.sensestreet.com\n  https: true\n  cert_subject: CN=www.sensestreet.com\n  cert_issued: Jul  7 21:38:41 2026 GMT\n  cert_expires: Oct  5 21:38:40 2026 GMT\n  cert_valid: true\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sensestreet.com\n  https: true\n  cert_subject: CN=docs.sensestreet.com\n  cert_issued: Jul  7 15:08:56 2026 GMT\n  cert_expires: Oct  5 15:08:55 2026 GMT\n  cert_valid: true\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.sensestreet.com\n  https: true\n  cert_subject: CN=sensestreet.com\n  cert_issuer: \"C=US, O=Let's Encrypt, CN=R13\"\n  cert_issued: Feb  2 08:31:24 2026 GMT\n  cert_expires: May  3 08:31:23 2026 GMT\n  cert_valid: false\n  finding: expired-certificate\n\
  \  finding_detail: >-\n    The customer-facing Sense Street portal — the host that also serves the live\n    /api/v1 surface — presents a Let's Encrypt certificate that expired on\n    2026-05-03, more than three months before this probe. curl refuses the\n    connection with exit 60 (certificate verify failed) and every browser will\n    interstitial. This is the single most material security finding on the\n    domain, and it is trivially fixable: the same wildcard was renewed on the\n    Framer-hosted marketing hosts but not here.\n  hsts: false\n  hsts_note: >-\n    No Strict-Transport-Security header on the portal, unlike the marketing and\n    docs hosts which both set max-age=31536000.\n  wildcard_sans:\n  - '*.api.sensestreet.com'\n  - '*.api.test.sensestreet.com'\n  - '*.auth.sensestreet.com'\n  - '*.aws.sensestreet.com'\n  - '*.ds.sensestreet.com'\n  - '*.gcp.sensestreet.com'\n  - '*.sensestreet.co.uk'\n  - '*.sensestreet.com'\n  - sensestreet.co.uk\n  - sensestreet.com\n  sans_note:\
  \ >-\n    The SAN list is itself a public disclosure of the deployment topology: a\n    per-tenant production API pattern (*.api.sensestreet.com), a matching test\n    environment (*.api.test.sensestreet.com), a separate auth surface\n    (*.auth.sensestreet.com), and both AWS and GCP delivery targets\n    (*.aws / *.gcp.sensestreet.com).\ndomains:\n- domain: sensestreet.com\n  dnssec: false\n  caa: []\n  caa_note: 'No CAA record — any public CA may issue for this domain.'\n  spf: true\n  spf_record: 'v=spf1 include:spf.protection.outlook.com ip4:20.90.220.112 -all'\n  spf_policy: hard-fail\n  dmarc: false\n  dmarc_note: >-\n    No _dmarc.sensestreet.com TXT record. SPF is published with a -all hard fail\n    but without DMARC there is no reporting and no policy applied to the header\n    From — a gap worth closing for a vendor whose customers are banks.\n  mx: sensestreet-com.mail.protection.outlook.com\nresolution_checks:\n- {host: api.sensestreet.com, result: NXDOMAIN, note: 'bare API\
  \ host does not resolve; tenants get a subdomain'}\n- {host: portal.sensestreet.com, result: 34.105.186.155}\n- {host: status.sensestreet.com, result: NXDOMAIN}\n- {host: trust.sensestreet.com, result: NXDOMAIN}\n- {host: developer.sensestreet.com, result: NXDOMAIN}\n- {host: mcp.sensestreet.com, result: NXDOMAIN}\nfindings:\n- {severity: high, id: expired-certificate, host: portal.sensestreet.com}\n- {severity: medium, id: no-dmarc, domain: sensestreet.com}\n- {severity: low, id: no-caa, domain: sensestreet.com}\n- {severity: low, id: no-dnssec, domain: sensestreet.com}\n- {severity: low, id: no-hsts-on-portal, host: portal.sensestreet.com}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sense-street/refs/heads/main/security/sense-street-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Capital Markets
- Trading
- Artificial Intelligence
- Fintech
- Conversation Intelligence
- OTC
- Market Data
- Natural Language Processing
- Commodities
- Fixed Income
---
