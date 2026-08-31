---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: world-kinect.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wfscorp.com
  note: DMARC reports route to tenant.admin@worldfuelservices.onmicrosoft.com.
  spf: true
hosts:
- cert_expires: Nov 13 04:09:42 2026 GMT
  host: www.world-kinect.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 21:34:29 2026 GMT
  host: auth.wfscorp.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_version: HTTP/2
  https: true
  note: OIDC issuer for the myWorld portal; serves /.well-known/openid-configuration.
- cert_expires: Nov  9 20:56:35 2026 GMT
  host: myworld.wfscorp.com
  hsts: false
  http_version: HTTP/2
  https: true
  note: Customer portal SPA. No Strict-Transport-Security header observed on the document response, and the host answers 200 with the SPA shell for every /.well-known/* path.
- host: www.world-fuel-services.com
  https: false
  note: DNS does not resolve (NXDOMAIN) — the domain in the previous apis.yml Website pointer.
kind: domain-security
layout: security
method: probed
name: World Fuel Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Fuel Services, probed live across 4 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: World Fuel Services
provider_slug: world-fuel-services
slug: world-fuel-services-domain-security
source_filename: world-fuel-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + brand hosts (2026-08-29)\nnote: >-\n  probe-domain-security.py covered the corporate host; auth.wfscorp.com (the Auth0-backed\n  identity host behind the myWorld customer portal) and myworld.wfscorp.com were probed by\n  hand in the same pass and appended here with their observed values. The legacy pointer host\n  www.world-fuel-services.com does not resolve at all (NXDOMAIN) and was removed from apis.yml.\nhosts:\n- host: www.world-kinect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 04:09:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: auth.wfscorp.com\n  https: true\n  http_version: HTTP/2\n  cert_expires: Nov 25 21:34:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: OIDC issuer for the myWorld portal; serves /.well-known/openid-configuration.\n- host: myworld.wfscorp.com\n  https: true\n  http_version: HTTP/2\n\
  \  cert_expires: Nov  9 20:56:35 2026 GMT\n  hsts: false\n  note: >-\n    Customer portal SPA. No Strict-Transport-Security header observed on the document\n    response, and the host answers 200 with the SPA shell for every /.well-known/* path.\n- host: www.world-fuel-services.com\n  https: false\n  note: DNS does not resolve (NXDOMAIN) — the domain in the previous apis.yml Website pointer.\ndomains:\n- domain: world-kinect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wfscorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: DMARC reports route to tenant.admin@worldfuelservices.onmicrosoft.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/world-fuel-services/refs/heads/main/security/world-fuel-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
- Energy
- Aviation Fuel
- Marine Fuel
- Fuel Distribution
- Energy Management
- Sustainability
- Logistics
- Fuel Cards
---
