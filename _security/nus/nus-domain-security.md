---
api_specs:
- filename: nus-identity-openapi.yml
  format: yaml
  label: NUS Federated Identity Service (VAFS)
  slug: identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/openapi/nus-identity-openapi.yml
description: 'Transport and domain security posture per host, with the operator recorded alongside. The organization field in each TLS certificate is the load-bearing column here: it is the hardest public evidence available of who actually runs a host, and it is what separates NUS''s own engineering from the platforms NUS rents.'
domains:
- caa: []
  dnssec: false
  domain: nus.edu.sg
  note: No DNSSEC and no CAA records on the institution's registrable domain.
hosts:
- a_record: 137.132.21.18
  cert_expires: Sep 25 23:59:59 2026 GMT
  cert_issuer: DigiCert EV RSA CA G2
  cert_subject_organization: National University of Singapore
  cert_validation: Extended Validation
  host: vafs.nus.edu.sg
  hsts: false
  https: true
  note: NUS's identity provider. EV certificate naming NUS as the validated organization (jurisdictionC=SG, businessCategory=Private Organization, serialNumber=200604346E). Negotiates TLS 1.2, not 1.3, and sends no HSTS header — weak for the host that fronts every credential in the university.
  tls_version: TLSv1.2
  x-operator: institution
- a_record: 137.132.173.15
  cert_expires: Oct 23 23:59:59 2026 GMT
  cert_issuer: Sectigo Public Server Authentication CA OV R36
  cert_subject_organization: National University of Singapore
  cert_validation: Organization Validation
  host: nnextbus.nus.edu.sg
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: NUS internal shuttle bus API. Live, HTTP Basic gated, CORS wide open (`*`).
  tls_version: TLSv1.2
  x-operator: institution
- a_record: 137.132.48.6
  cert_expires: Dec 19 23:59:59 2026 GMT
  cert_issuer: Sectigo Public Server Authentication CA OV R36
  cert_subject_organization: National University of Singapore
  cert_validation: Organization Validation
  host: api.nus.edu.sg
  hsts: false
  https: true
  note: API gateway hostname on an NUS-issued certificate that returns HTTP 500 on every probed path. Live host, no service.
  x-operator: institution
- a_record: 137.132.7.240
  cert_subject_organization: National University of Singapore
  host: luminus.nus.edu.sg
  https: true
  note: Decommissioned in-house learning management system. DNS and certificate still present; the host does not complete a connection. Recorded as a dead host, not a surface.
  reachable: false
  x-operator: institution
- cert_expires: Sep 29 02:20:51 2026 GMT
  host: nus.edu.sg
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Main web estate behind Imperva. Answers unknown paths with HTTP 200 and an HTML body, so /llms.txt and /robots.txt both soft-404. Neither artifact exists.
  tls_version: TLSv1.3
  waf: Imperva/Incapsula
  x-operator: institution
- cert_expires: Oct  5 06:49:35 2026 GMT
  cname: nusor.cname.openrepository.com
  host: scholarbank.nus.edu.sg
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Institutional repository. The CNAME to openrepository.com is the operator evidence — Atmire Open Repository hosts and runs the DSpace 7.6 instance.
  tls_version: TLSv1.3
  x-operator: tenant
- cert_subject_organization: null
  cert_validation: Domain Validation
  cname: nus-vanity.instructure.com
  host: canvas.nus.edu.sg
  https: true
  note: Canvas LMS tenant. Certificate carries no organization — issued by the platform, not NUS.
  x-operator: tenant
- cert_expires: Sep 27 08:32:54 2026 GMT
  cert_issuer: Let's Encrypt
  cert_subject_organization: null
  cname: c1141.campuspress.com
  host: blog.nus.edu.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: NUS blogs platform on CampusPress managed WordPress.
  x-operator: tenant
- cname: region-au.libguides.com
  host: libguides.nus.edu.sg
  https: true
  note: Springshare LibGuides tenant, served from the Australian region.
  x-operator: tenant
- cname: nus.iii.com
  host: linc.nus.edu.sg
  https: true
  note: Innovative Interfaces library catalogue tenant. Bot-challenged from this network.
  x-operator: tenant
- cert_expires: Sep  4 03:57:51 2026 GMT
  host: api.nusmods.com
  hsts: false
  https: true
  note: NUSMods, run by the NUSModifications student organisation behind Cloudflare. Not an NUS host and not on an NUS domain; listed because it is where NUS course data is publicly readable.
  tls_version: TLSv1.3
  x-operator: tenant
kind: domain-security
layout: security
method: probed
name: Nus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National University of Singapore, probed live across 11 host(s) and 1 registrable domain(s). 11 host(s) serve HTTPS (up to TLSv1.2); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: National University of Singapore
provider_slug: nus
slug: nus-domain-security
source_filename: nus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every host in apis.yml, 2026-08-19\ndescription: >-\n  Transport and domain security posture per host, with the operator recorded alongside. The\n  organization field in each TLS certificate is the load-bearing column here: it is the hardest\n  public evidence available of who actually runs a host, and it is what separates NUS's own\n  engineering from the platforms NUS rents.\nhosts:\n- host: vafs.nus.edu.sg\n  x-operator: institution\n  https: true\n  tls_version: TLSv1.2\n  cert_subject_organization: National University of Singapore\n  cert_validation: Extended Validation\n  cert_issuer: DigiCert EV RSA CA G2\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  a_record: 137.132.21.18\n  hsts: false\n  note: >-\n    NUS's identity provider. EV certificate naming NUS as the validated organization\n    (jurisdictionC=SG, businessCategory=Private Organization, serialNumber=200604346E).\n    Negotiates TLS\
  \ 1.2, not 1.3, and sends no HSTS header — weak for the host that fronts every\n    credential in the university.\n- host: nnextbus.nus.edu.sg\n  x-operator: institution\n  https: true\n  tls_version: TLSv1.2\n  cert_subject_organization: National University of Singapore\n  cert_validation: Organization Validation\n  cert_issuer: Sectigo Public Server Authentication CA OV R36\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  a_record: 137.132.173.15\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: NUS internal shuttle bus API. Live, HTTP Basic gated, CORS wide open (`*`).\n- host: api.nus.edu.sg\n  x-operator: institution\n  https: true\n  cert_subject_organization: National University of Singapore\n  cert_validation: Organization Validation\n  cert_issuer: Sectigo Public Server Authentication CA OV R36\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  a_record: 137.132.48.6\n  hsts: false\n  note: >-\n    API gateway hostname on an NUS-issued certificate that returns\
  \ HTTP 500 on every probed\n    path. Live host, no service.\n- host: luminus.nus.edu.sg\n  x-operator: institution\n  https: true\n  cert_subject_organization: National University of Singapore\n  a_record: 137.132.7.240\n  reachable: false\n  note: >-\n    Decommissioned in-house learning management system. DNS and certificate still present; the\n    host does not complete a connection. Recorded as a dead host, not a surface.\n- host: nus.edu.sg\n  x-operator: institution\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:20:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  waf: Imperva/Incapsula\n  note: >-\n    Main web estate behind Imperva. Answers unknown paths with HTTP 200 and an HTML body, so\n    /llms.txt and /robots.txt both soft-404. Neither artifact exists.\n- host: scholarbank.nus.edu.sg\n  x-operator: tenant\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 06:49:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  cname: nusor.cname.openrepository.com\n\
  \  note: >-\n    Institutional repository. The CNAME to openrepository.com is the operator evidence — Atmire\n    Open Repository hosts and runs the DSpace 7.6 instance.\n- host: canvas.nus.edu.sg\n  x-operator: tenant\n  https: true\n  cert_subject_organization: null\n  cert_validation: Domain Validation\n  cname: nus-vanity.instructure.com\n  note: Canvas LMS tenant. Certificate carries no organization — issued by the platform, not NUS.\n- host: blog.nus.edu.sg\n  x-operator: tenant\n  https: true\n  cert_subject_organization: null\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep 27 08:32:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  cname: c1141.campuspress.com\n  note: NUS blogs platform on CampusPress managed WordPress.\n- host: libguides.nus.edu.sg\n  x-operator: tenant\n  https: true\n  cname: region-au.libguides.com\n  note: Springshare LibGuides tenant, served from the Australian region.\n- host: linc.nus.edu.sg\n  x-operator: tenant\n  https: true\n  cname: nus.iii.com\n\
  \  note: Innovative Interfaces library catalogue tenant. Bot-challenged from this network.\n- host: api.nusmods.com\n  x-operator: tenant\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:57:51 2026 GMT\n  hsts: false\n  note: >-\n    NUSMods, run by the NUSModifications student organisation behind Cloudflare. Not an NUS\n    host and not on an NUS domain; listed because it is where NUS course data is publicly\n    readable.\ndomains:\n- domain: nus.edu.sg\n  dnssec: false\n  caa: []\n  note: No DNSSEC and no CAA records on the institution's registrable domain.\nobservations:\n- >-\n  Every host NUS actually runs (vafs, nnextbus, api, luminus) carries a certificate naming\n  National University of Singapore as the organization. Every host NUS rents carries either no\n  organization or the platform's. This one field settles operator attribution more reliably than\n  any heuristic.\n- >-\n  The identity provider — the highest-value host in the estate — has the weakest transport\n\
  \  posture of the institution-operated set: TLS 1.2 only and no HSTS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/security/nus-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- University
- Higher Education
- Education
- Singapore
- Research
- Identity Federation
- Research Repository
- Course Catalog
- Open Access
- Learning Management
---
