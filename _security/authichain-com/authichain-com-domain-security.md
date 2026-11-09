---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: authichain.com
  spf: true
hosts:
- cert_expires: Jan 30 19:22:56 2027 GMT
  host: authichain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Authichain Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AuthiChain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AuthiChain
provider_slug: authichain-com
slug: authichain-com-domain-security
source_filename: authichain-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: authichain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 19:22:56 2027 GMT\n  hsts: false\ndomains:\n- domain: authichain.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/authichain-com/security/authichain-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Verification
- QR
- Digital Product Passport
- Supply Chain
---
