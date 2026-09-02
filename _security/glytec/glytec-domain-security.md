---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: glytec.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: glytecsystems.com
  spf: true
hosts:
- cert_expires: Oct 20 20:03:50 2026 GMT
  host: glytec.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: app.glytec.com
  hsts: null
  https: true
  notes: GlytecOne Command Center tenant login (organization-scoped). Root returns 302 into the login flow. Fronted by an AWS ELB (k8s-prod01cluster-*.us-east-2.elb.amazonaws.com).
  tls_version: TLSv1.2
- cert_expires: Oct  7 20:24:14 2026 GMT
  host: glytecsystems.com
  hsts: null
  https: true
  notes: Legacy corporate domain; 301 redirects to https://glytec.com/.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glytec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glytec, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Glytec
provider_slug: glytec
slug: glytec-domain-security
source_filename: glytec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + application hosts\nhosts:\n- host: glytec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 20:03:50 2026 GMT\n  hsts: null\n- host: app.glytec.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: null\n  notes: >-\n    GlytecOne Command Center tenant login (organization-scoped). Root returns 302 into the login flow.\n    Fronted by an AWS ELB (k8s-prod01cluster-*.us-east-2.elb.amazonaws.com).\n- host: glytecsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:24:14 2026 GMT\n  hsts: null\n  notes: Legacy corporate domain; 301 redirects to https://glytec.com/.\ndomains:\n- domain: glytec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: glytecsystems.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n\
  findings:\n- No HSTS response header observed on any Glytec host.\n- No CAA record on glytec.com; glytecsystems.com pins issuance to letsencrypt.org.\n- DNSSEC not enabled on either registrable domain.\n- DMARC published at p=quarantine on both domains (glytecsystems.com sets sp=none for subdomains).\n- No /.well-known/security.txt on any host, so no machine-readable security contact is advertised.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glytec/refs/heads/main/security/glytec-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health IT
- Clinical Decision Support
- Diabetes
- Insulin Management
- glycemic-management
- Hospital
- EHR Integration
- HL7
- Medical Device
- Software as a Medical Device
---
