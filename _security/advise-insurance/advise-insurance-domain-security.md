---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bloomthrives.com
  notes:
  - 'SPF re-probed by hand 2026-09-09 after the scripted dig returned an empty TXT set on the first try; the apex publishes a v=spf1 record ending -all. Note the record begins Ip4: (capital I) on the first mechanism, which some strict parsers reject.'
  - A stray v=DMARC1; p=reject; adkim=s; aspf=s TXT record is published at the APEX (bloomthrives.com) in addition to the correct one at _dmarc.bloomthrives.com (p=quarantine; pct=100). Apex DMARC records are not read by receivers; the effective policy is quarantine.
  - No DNSKEY and no CAA records observed for bloomthrives.com.
  spf: true
  spf_record: v=spf1 Ip4:66.244.115.1 ip4:66.244.115.241 ip4:66.244.115.242 ip4:65.111.246.2 ip4:65.111.246.3 include:spf.protection.outlook.com -all
hosts:
- cert_expires: Nov 26 09:46:38 2026 GMT
  host: www.bloomthrives.com
  hsts: true
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Advise Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advise Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Advise Insurance
provider_slug: advise-insurance
slug: advise-insurance-domain-security
source_filename: advise-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomthrives.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 09:46:38 2026 GMT\n  hsts: true\ndomains:\n- domain: bloomthrives.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 Ip4:66.244.115.1 ip4:66.244.115.241 ip4:66.244.115.242 ip4:65.111.246.2 ip4:65.111.246.3 include:spf.protection.outlook.com -all'\n  dmarc: true\n  dmarc_policy: quarantine\n  notes:\n  - 'SPF re-probed by hand 2026-09-09 after the scripted dig returned an empty TXT\n    set on the first try; the apex publishes a v=spf1 record ending -all. Note the\n    record begins Ip4: (capital I) on the first mechanism, which some strict parsers\n    reject.'\n  - 'A stray v=DMARC1; p=reject; adkim=s; aspf=s TXT record is published at the APEX\n    (bloomthrives.com) in addition to the correct one at _dmarc.bloomthrives.com\n    (p=quarantine; pct=100). Apex\
  \ DMARC records are not read by receivers; the\n    effective policy is quarantine.'\n  - 'No DNSKEY and no CAA records observed for bloomthrives.com.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advise-insurance/refs/heads/main/security/advise-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Health Insurance
- Medicare
- Health Care
- Insurtech
- Enrollment
- Telesales
---
