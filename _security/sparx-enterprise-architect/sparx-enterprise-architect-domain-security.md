---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sparxsystems.com
  spf: true
hosts:
- cert_expires: Sep 27 03:19:08 2026 GMT
  host: sparxsystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sparx Enterprise Architect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sparx Enterprise Architect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sparx Enterprise Architect
provider_slug: sparx-enterprise-architect
slug: sparx-enterprise-architect-domain-security
source_filename: sparx-enterprise-architect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sparxsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:19:08 2026 GMT\n  hsts: false\ndomains:\n- domain: sparxsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparx-enterprise-architect/refs/heads/main/security/sparx-enterprise-architect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Enterprise Architecture
- Modeling
- Software Engineering
- Systems Engineering
- UML
---
