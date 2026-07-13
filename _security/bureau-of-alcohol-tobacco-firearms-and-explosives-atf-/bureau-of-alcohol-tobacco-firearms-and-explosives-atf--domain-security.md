---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: atf.gov
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: www.atf.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bureau Of Alcohol Tobacco Firearms And Explosives Atf  Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Alcohol, Tobacco, Firearms and Explosives (ATF), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Alcohol, Tobacco, Firearms and Explosives (ATF)
provider_slug: bureau-of-alcohol-tobacco-firearms-and-explosives-atf-
slug: bureau-of-alcohol-tobacco-firearms-and-explosives-atf--domain-security
source_filename: bureau-of-alcohol-tobacco-firearms-and-explosives-atf--domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atf.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: atf.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-alcohol-tobacco-firearms-and-explosives-atf-/refs/heads/main/security/bureau-of-alcohol-tobacco-firearms-and-explosives-atf--domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Alcohol
- Explosives
- Federal Government
- Firearms
- Law Enforcement
- Public Safety
- Tobacco
---
