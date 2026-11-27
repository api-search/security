---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chainoftitle.org
  spf: true
hosts:
- cert_expires: Dec  6 00:25:18 2026 GMT
  host: chainoftitle.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chain of Title Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chain of Title, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chain of Title
provider_slug: chainoftitle-org
slug: chainoftitle-org-domain-security
source_filename: chainoftitle-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chainoftitle.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 00:25:18 2026 GMT\n  hsts: false\ndomains:\n- domain: chainoftitle.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chainoftitle-org/security/chainoftitle-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Blockchain
- Solana
- Tokens
- Provenance
- Company
---
