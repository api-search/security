---
api_specs:
- filename: piscescsm-openapi.yml
  format: yaml
  label: piscesCSM
  slug: piscescsm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/piscescsm/refs/heads/main/openapi/piscescsm-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:certificates@uq.edu.au"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uq.edu.au
  spf: true
hosts:
- cert_expires: Jul 18 12:42:29 2026 GMT
  host: biosig.lab.uq.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Piscescsm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for piscesCSM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: piscesCSM
provider_slug: piscescsm
slug: piscescsm-domain-security
source_filename: piscescsm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biosig.lab.uq.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 18 12:42:29 2026 GMT\n  hsts: false\ndomains:\n- domain: uq.edu.au\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:certificates@uq.edu.au\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/piscescsm/refs/heads/main/security/piscescsm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Bioinformatics
- Drug Discovery
- Cancer
---
