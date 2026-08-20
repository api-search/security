---
api_specs:
- filename: tigera-apis-api-openapi.yml
  format: yaml
  label: Tigera APIS API
  slug: tigera-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-apis-api-openapi.yml
- filename: tigera-projectcalicoorg-api-openapi.yml
  format: yaml
  label: Tigera Projectcalico Org API
  slug: tigera-projectcalicoorg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-projectcalicoorg-api-openapi.yml
- filename: tigera-projectcalicoorg-v3-api-openapi.yml
  format: yaml
  label: Tigera Projectcalico Org V3 API
  slug: tigera-projectcalicoorg-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-projectcalicoorg-v3-api-openapi.yml
- filename: tigera-version-api-openapi.yml
  format: yaml
  label: Tigera Version API
  slug: tigera-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-version-api-openapi.yml
description: TLS/HSTS posture per host and DNS security records per registrable domain. Both public domains (tigera.io, calicocloud.io) publish SPF and a DMARC policy of p=reject; neither publishes DS records, so DNSSEC is not signed. tigera.io publishes no CAA record; calicocloud.io does, restricting issuance to Google Trust Services, DigiCert and Let's Encrypt. Every reachable host negotiates TLS 1.3 with HSTS at one year or more, and status.calicocloud.io is preload-eligible.
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tigera.io
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: calicocloud.io
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net ~all
hosts:
- cert_expires: Sep 25 23:57:44 2026 GMT
  host: www.tigera.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 17:43:43 2026 GMT
  host: docs.tigera.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 10:38:31 2026 GMT
  host: www.calicocloud.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: status.calicocloud.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63113904
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- host: api.calicocloud.io
  https: false
  note: Probed as a candidate Calico Cloud API host; no DNS A record exists.
  reason: dns-nxdomain
kind: domain-security
layout: security
method: probed
name: Tigera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tigera, probed live across 5 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tigera
provider_slug: tigera
slug: tigera-domain-security
source_filename: tigera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\ndescription: >-\n  TLS/HSTS posture per host and DNS security records per registrable domain. Both public domains\n  (tigera.io, calicocloud.io) publish SPF and a DMARC policy of p=reject; neither publishes DS\n  records, so DNSSEC is not signed. tigera.io publishes no CAA record; calicocloud.io does,\n  restricting issuance to Google Trust Services, DigiCert and Let's Encrypt. Every reachable\n  host negotiates TLS 1.3 with HSTS at one year or more, and status.calicocloud.io is\n  preload-eligible.\nhosts:\n- host: www.tigera.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:57:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tigera.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:43:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.calicocloud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires:\
  \ Sep 19 10:38:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: status.calicocloud.io\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63113904\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: api.calicocloud.io\n  https: false\n  reason: dns-nxdomain\n  note: Probed as a candidate Calico Cloud API host; no DNS A record exists.\nnot_probed:\n- host: kubernetes.default.svc\n  reason: >-\n    In-cluster Kubernetes service address for the Calico aggregated API server. Not a public\n    host — there is nothing on the internet to probe, and its TLS is the customer's own cluster\n    CA.\n- host: goldmane.calico-system.svc\n  reason: In-cluster service address for the Goldmane flows service; same as above.\ndomains:\n- domain: tigera.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: calicocloud.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\
  \n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net ~all\n  dmarc: true\n  dmarc_policy: reject\nx-evidence:\n  fetched: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/security/tigera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Kubernetes
- Networking
- Network Security
- Container Security
- Cloud-Native
- Observability
- Microsegmentation
- Zero Trust
- eBPF
- Open-Source
---
