---
description: ''
domains:
- a_records:
  - 141.193.213.20
  - 141.193.213.21
  caa: []
  created: '2018-01-06'
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: inboundhealth.com
  last_updated: '2026-01-07'
  mail_still_routed: true
  mx:
  - inboundhealth-com.mail.protection.outlook.com
  nameservers:
  - ns15.domaincontrol.com
  - ns16.domaincontrol.com
  registrar: GoDaddy.com, LLC
  registry_expiry: '2027-01-06'
  spf: true
  spf_defect: TWO v=spf1 TXT records are published on the same domain. RFC 7208 s3.2 requires exactly one; a receiver that finds more than one MUST return permerror, so SPF evaluation for this domain fails outright. The two records also disagree on the qualifier (-all vs ~all).
  spf_records:
  - v=spf1 include:spf.protection.outlook.com include:spf.loxo.co -all
  - v=spf1 include:_spf.brightmove.com ~all
hosts:
- cert_expires: Oct 18 18:52:07 2026 GMT
  cert_issuer: Google Trust Services WE1
  edge: cloudflare
  host: inboundhealth.com
  hsts: false
  http_status: 526
  https: true
  origin_reachable: false
  referrer_policy: same-origin
  tls_version: TLSv1.3
  x_frame_options: SAMEORIGIN
- cert_expires: Oct 17 22:40:45 2026 GMT
  cert_issuer: Google Trust Services WE1
  edge: cloudflare
  host: www.inboundhealth.com
  hsts: false
  http_status: 526
  https: true
  origin_reachable: false
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inbound Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inbound Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Inbound Health
provider_slug: inbound-health
slug: inbound-health-domain-security
source_filename: inbound-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: dig + TLS handshake + HTTP HEAD against inboundhealth.com, 2026-08-23\nnote: >-\n  Probed after the company ceased operations (December 2025). The domain is retained and the\n  Cloudflare edge still terminates TLS with a valid certificate, but the origin is gone, so every\n  HTTPS request ends in a Cloudflare 526. Mail is still routed to Microsoft 365, which is why the\n  DNS zone is still being maintained. Recorded as evidence of a retained-but-dead domain, not as\n  evidence of a live API host.\nhosts:\n- host: inboundhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services WE1\n  cert_expires: 'Oct 18 18:52:07 2026 GMT'\n  edge: cloudflare\n  origin_reachable: false\n  http_status: 526\n  hsts: false\n  x_frame_options: SAMEORIGIN\n  referrer_policy: same-origin\n- host: www.inboundhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services WE1\n  cert_expires: 'Oct\
  \ 17 22:40:45 2026 GMT'\n  edge: cloudflare\n  origin_reachable: false\n  http_status: 526\n  hsts: false\ndomains:\n- domain: inboundhealth.com\n  registrar: GoDaddy.com, LLC\n  created: '2018-01-06'\n  registry_expiry: '2027-01-06'\n  last_updated: '2026-01-07'\n  nameservers: [ns15.domaincontrol.com, ns16.domaincontrol.com]\n  a_records: [141.193.213.20, 141.193.213.21]\n  dnssec: false\n  caa: []\n  spf: true\n  spf_records:\n  - 'v=spf1 include:spf.protection.outlook.com include:spf.loxo.co -all'\n  - 'v=spf1 include:_spf.brightmove.com ~all'\n  spf_defect: >-\n    TWO v=spf1 TXT records are published on the same domain. RFC 7208 s3.2 requires exactly one;\n    a receiver that finds more than one MUST return permerror, so SPF evaluation for this domain\n    fails outright. The two records also disagree on the qualifier (-all vs ~all).\n  dmarc: false\n  dmarc_policy: null\n  mx: [inboundhealth-com.mail.protection.outlook.com]\n  mail_still_routed: true\nfindings:\n- id: origin-down\n\
  \  detail: All HTTPS paths return Cloudflare 526; the site has no reachable origin.\n- id: no-dnssec\n  detail: No DNSKEY record published.\n- id: no-caa\n  detail: No CAA record; certificate issuance is unconstrained.\n- id: no-dmarc\n  detail: No _dmarc TXT record, so no policy governs mail claiming to be from this domain.\n- id: duplicate-spf\n  detail: Two conflicting v=spf1 records make SPF permerror for the whole domain.\n- id: no-hsts\n  detail: No Strict-Transport-Security header on the edge response.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inbound-health/refs/heads/main/security/inbound-health-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Defunct
- Healthcare
- Hospital-at-Home
- Home Health
- Remote Patient Monitoring
- Value-Based Care
- Care Coordination
- Health Systems
- Digital Health
---
