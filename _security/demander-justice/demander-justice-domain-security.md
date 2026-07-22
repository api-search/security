---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: demanderjustice.com
  spf: true
hosts:
- cert_expires: Oct 10 21:48:53 2026 GMT
  host: demanderjustice.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Demander Justice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Demander Justice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Demander Justice
provider_slug: demander-justice
slug: demander-justice-domain-security
source_filename: demander-justice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: demanderjustice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 21:48:53 2026 GMT\n  hsts: false\ndomains:\n- domain: demanderjustice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demander-justice/refs/heads/main/security/demander-justice-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Legal
- LegalTech
- Justice
- Dispute Resolution
- France
- Access to Justice
---
