---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dstl.gov.uk
  spf: true
hosts:
- host: www.dstl.gov.uk
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.dstl.go'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Defence Science Technology Laboratories Dstl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defence Science & Technology Laboratories (Dstl), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Defence Science & Technology Laboratories (Dstl)
provider_slug: defence-science-technology-laboratories-dstl
slug: defence-science-technology-laboratories-dstl-domain-security
source_filename: defence-science-technology-laboratories-dstl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dstl.gov.uk\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.dstl.go'\n  hsts: null\ndomains:\n- domain: dstl.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/defence-science-technology-laboratories-dstl/security/defence-science-technology-laboratories-dstl-domain-security.yml
summary_line: DMARC
tags:
- defence
- research
- technology
- government
- UK
---
