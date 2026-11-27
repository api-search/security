---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: companystack.co.uk
  spf: true
hosts:
- cert_expires: Jan  5 22:17:23 2027 GMT
  host: companystack.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CompanyStack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompanyStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CompanyStack
provider_slug: companystack-co-uk
slug: companystack-co-uk-domain-security
source_filename: companystack-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: companystack.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 22:17:23 2027 GMT\n  hsts: null\ndomains:\n- domain: companystack.co.uk\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/companystack-co-uk/security/companystack-co-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Company Data
- Companies House
- United Kingdom
- KYB
- Business Verification
- MCP
---
