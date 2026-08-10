---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dnanexus.com
  spf: true
hosts:
- cert_expires: Sep 28 10:04:06 2026 GMT
  host: www.dnanexus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 06:19:01 2026 GMT
  host: documentation.dnanexus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 15:48:59 2026 GMT
  host: api.dnanexus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dnanexus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNAnexus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DNAnexus
provider_slug: dnanexus
slug: dnanexus-domain-security
source_filename: dnanexus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dnanexus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:04:06 2026 GMT\n  hsts: null\n- host: documentation.dnanexus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 06:19:01 2026 GMT\n  hsts: null\n- host: api.dnanexus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 15:48:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dnanexus.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnanexus/refs/heads/main/security/dnanexus-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Genomics
- Bioinformatics
- Life Sciences
- Healthcare
- Cloud Computing
- Data Platform
- Scientific Computing
- Precision Medicine
- Clinical Research
---
