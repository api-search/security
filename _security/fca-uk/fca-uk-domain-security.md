---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fca.org.uk
  spf: true
hosts:
- cert_expires: Oct 15 15:48:44 2026 GMT
  host: www.fca.org.uk
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 16:23:17 2026 GMT
  host: register.fca.org.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fca Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Financial Conduct Authority, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Financial Conduct Authority
provider_slug: fca-uk
slug: fca-uk-domain-security
source_filename: fca-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fca.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:48:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: register.fca.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 16:23:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fca.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fca-uk/refs/heads/main/security/fca-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- United Kingdom
- Regulator
- Market Infrastructure
- Financial Services
- Public Register
- Conduct Regulation
- Open Finance
- Insurance Intermediaries
- Risk Data
- Market Data
- Reference Data
- MiFID II
---
