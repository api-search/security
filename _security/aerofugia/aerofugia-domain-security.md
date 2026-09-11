---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aerofugia.com
  mx: geely.com / Microsoft 365 (mx-inbound.geely.com, geely-com.mail.protection.outlook.com)
  note: Mail and SPF are delegated to parent Geely; no _dmarc TXT record exists, and the apex publishes no A record, no CAA and no DNSKEY.
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:spf.geely.com -all
hosts:
- cert_expires: Dec 18 09:01:42 2026 GMT
  host: www.aerofugia.com
  hsts: false
  https: true
  note: 'The root document (HTTP 200) carries no Strict-Transport-Security header; the only responses that do are the nginx 301s served for /api* paths, which redirect to themselves. www is the entire web surface: the apex aerofugia.com publishes no A record.'
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aerofugia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aerofugia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aerofugia
provider_slug: aerofugia
slug: aerofugia-domain-security
source_filename: aerofugia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (probe-domain-security.py), enriched by hand\n  from the same 2026-09-10 probe session\nhosts:\n- host: www.aerofugia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 09:01:42 2026 GMT\n  hsts: false\n  note: 'The root document (HTTP 200) carries no Strict-Transport-Security header; the only responses\n    that do are the nginx 301s served for /api* paths, which redirect to themselves. www is the entire\n    web surface: the apex aerofugia.com publishes no A record.'\ndomains:\n- domain: aerofugia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  mx: geely.com / Microsoft 365 (mx-inbound.geely.com, geely-com.mail.protection.outlook.com)\n  spf_record: v=spf1 include:spf.protection.outlook.com include:spf.geely.com -all\n  note: 'Mail and SPF are delegated to parent Geely; no _dmarc TXT record exists, and the apex publishes\n    no A record, no\
  \ CAA and no DNSKEY.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerofugia/refs/heads/main/security/aerofugia-domain-security.yml
summary_line: TLSv1.3
tags:
- Aviation
- Aerospace
- eVTOL
- Advanced Air Mobility
- Urban Air Mobility
- Electric Aircraft
- Transportation
- Manufacturing
- China
- Company
---
