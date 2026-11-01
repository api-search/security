---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avalotx.com
  spf: true
hosts:
- cert_expires: Nov 30 03:54:59 2026 GMT
  host: www.avalotx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cerecor Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cerecor Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cerecor Inc.
provider_slug: cerecor-inc
slug: cerecor-inc-domain-security
source_filename: cerecor-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avalotx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 03:54:59 2026 GMT\n  hsts: false\ndomains:\n- domain: avalotx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cerecor-inc/security/cerecor-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Therapeutics
- IL-1β
- Clinical-stage
---
