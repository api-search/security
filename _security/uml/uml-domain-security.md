---
api_specs:
- filename: plantuml-server-openapi.yml
  format: yaml
  label: PlantUML Server API
  slug: plantuml-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uml/refs/heads/main/openapi/plantuml-server-openapi.yml
- filename: kroki-openapi.yml
  format: yaml
  label: Kroki Diagram API
  slug: kroki
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uml/refs/heads/main/openapi/kroki-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: omg.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: plantuml.com
  spf: false
hosts:
- cert_expires: Aug 16 05:03:03 2026 GMT
  host: www.omg.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:43:46 2026 GMT
  host: plantuml.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 15:46:23 2026 GMT
  host: www.plantuml.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UML, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UML
provider_slug: uml
slug: uml-domain-security
source_filename: uml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omg.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 05:03:03 2026 GMT\n  hsts: false\n- host: plantuml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:43:46 2026 GMT\n  hsts: false\n- host: www.plantuml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:46:23 2026 GMT\n  hsts: false\ndomains:\n- domain: omg.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: plantuml.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uml/refs/heads/main/security/uml-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- UML
- Modeling
- Diagrams
- Software Architecture
- Design
- Standards
---
