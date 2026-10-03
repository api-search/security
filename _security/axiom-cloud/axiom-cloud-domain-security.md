---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: axiom.trade
  spf: true
hosts:
- cert_expires: Dec  3 20:44:10 2026 GMT
  host: axiom.trade
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axiom Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiom Cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Axiom Cloud
provider_slug: axiom-cloud
slug: axiom-cloud-domain-security
source_filename: axiom-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axiom.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 20:44:10 2026 GMT\n  hsts: null\ndomains:\n- domain: axiom.trade\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axiom-cloud/refs/heads/main/security/axiom-cloud-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Trading
- Fintech
---
