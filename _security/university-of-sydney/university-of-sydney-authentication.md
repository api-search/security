---
api_key_in: []
auth_types: []
description: 'The University of Sydney publishes no public API authentication scheme, because it publishes no public API. What it does operate — and what is genuinely machine-readable — is federated identity: a Shibboleth SAML 2.0 identity provider registered in the Australian Access Federation and republished into eduGAIN, plus an Okta tenant fronting web application sign-in. Every application surface reachable from the public internet redirects into one of these two.'
kind: authentication
layout: security
method: probed
name: University Of Sydney Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Sydney declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: University of Sydney
provider_slug: university-of-sydney
scheme_count: 4
schemes:
- audience: Staff, students and federated research services. Relying parties must be registered service providers in AAF or eduGAIN; there is no self-service registration for third-party developers.
  bindings:
  - https://federation.sydney.edu.au/idp/profile/SAML2/Redirect/SSO
  - https://federation.sydney.edu.au/idp/profile/SAML2/POST/SSO
  - https://federation.sydney.edu.au/idp/profile/SAML2/POST-SimpleSign/SSO
  entityId: https://federation.sydney.edu.au/idp/shibboleth
  federations:
  - metadata: https://md.aaf.edu.au/aaf-metadata.xml
    name: Australian Access Federation
    status: 200
  - metadata: https://mds.edugain.org/edugain-v2.xml
    name: eduGAIN
    status: 200
  hosting: federation.sydney.edu.au CNAMEs to d007b274d34f1a4319cafeaf6941cfa7.idp-cname.aaf.edu.au, served through CloudFront and an AWS ALB by Jetty 12.1.0 under an Amazon-issued certificate. AAF operates the identity-provider software; the University of Sydney owns the entity, the scope sydney.edu.au and the SAML signing key.
  id: saml2-shibboleth-idp
  metadataUrl: https://federation.sydney.edu.au/idp/shibboleth
  name: SAML 2.0 / Shibboleth (Australian Access Federation)
  operator: tenant
  protocols:
  - urn:oasis:names:tc:SAML:2.0:protocol
  scope: sydney.edu.au
  type: federated-identity
  vendor: Australian Access Federation (Rapid IdP)
  verified: '2026-08-19'
- detail: sso.sydney.edu.au is a vanity hostname CNAMEd to the institution's Okta tenant. It brokers sign-in for institution web applications; canvas.sydney.edu.au redirects into it with a SAMLRequest. The contract is Okta's, the tenant is the university's.
  host: sso.sydney.edu.au
  id: okta-web-sso
  name: Okta hosted sign-in (institution tenant)
  operator: tenant
  resolves: sydneyuni.customdomains.okta.com
  type: oidc-saml-broker
  verified: '2026-08-19'
- detail: The myUni student portal is backed by internal JSON endpoints consumed by the authenticated single-page application. They require an established student session, are not documented, and are not offered to third-party developers.
  hosts:
  - myuni.sydney.edu.au
  id: session-gated-app-apis
  name: Session-gated application APIs
  operator: institution
  type: session-cookie
  verified: '2026-08-19'
- detail: Alma and Primo API keys covering the university's library data are issued by Ex Libris to the institution through the Ex Libris Developer Network. The university does not publish or re-issue them.
  id: vendor-issued-api-keys
  issuer: https://developers.exlibrisgroup.com/
  name: Vendor-issued API keys (Ex Libris)
  operator: vendor
  type: api-key
slug: university-of-sydney-authentication
source_filename: university-of-sydney-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: University of Sydney\nproviderId: university-of-sydney\ngenerated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live fetch of https://federation.sydney.edu.au/idp/shibboleth, the Australian Access\n  Federation metadata aggregate, the eduGAIN metadata aggregate, and DNS/redirect tracing of\n  canvas.sydney.edu.au, sso.sydney.edu.au and myuni.sydney.edu.au.\ndescription: >-\n  The University of Sydney publishes no public API authentication scheme, because it publishes\n  no public API. What it does operate — and what is genuinely machine-readable — is federated\n  identity: a Shibboleth SAML 2.0 identity provider registered in the Australian Access\n  Federation and republished into eduGAIN, plus an Okta tenant fronting web application sign-in.\n  Every application surface reachable from the public internet redirects into one of these two.\nnotes: >-\n  No OAuth 2.0 authorization server, no API\
  \ key issuance process, and no developer credential\n  self-service was found on any institution host. Ex Libris Alma/Primo API keys for the\n  library platform are issued by the vendor through the Ex Libris Developer Network, not by\n  the university.\nschemes:\n- id: saml2-shibboleth-idp\n  name: SAML 2.0 / Shibboleth (Australian Access Federation)\n  type: federated-identity\n  operator: tenant\n  vendor: Australian Access Federation (Rapid IdP)\n  hosting: >-\n    federation.sydney.edu.au CNAMEs to d007b274d34f1a4319cafeaf6941cfa7.idp-cname.aaf.edu.au,\n    served through CloudFront and an AWS ALB by Jetty 12.1.0 under an Amazon-issued certificate.\n    AAF operates the identity-provider software; the University of Sydney owns the entity, the\n    scope sydney.edu.au and the SAML signing key.\n  metadataUrl: https://federation.sydney.edu.au/idp/shibboleth\n  entityId: https://federation.sydney.edu.au/idp/shibboleth\n  scope: sydney.edu.au\n  protocols:\n  - urn:oasis:names:tc:SAML:2.0:protocol\n\
  \  bindings:\n  - https://federation.sydney.edu.au/idp/profile/SAML2/Redirect/SSO\n  - https://federation.sydney.edu.au/idp/profile/SAML2/POST/SSO\n  - https://federation.sydney.edu.au/idp/profile/SAML2/POST-SimpleSign/SSO\n  federations:\n  - name: Australian Access Federation\n    metadata: https://md.aaf.edu.au/aaf-metadata.xml\n    status: 200\n  - name: eduGAIN\n    metadata: https://mds.edugain.org/edugain-v2.xml\n    status: 200\n  audience: >-\n    Staff, students and federated research services. Relying parties must be registered\n    service providers in AAF or eduGAIN; there is no self-service registration for third-party\n    developers.\n  verified: '2026-08-19'\n- id: okta-web-sso\n  name: Okta hosted sign-in (institution tenant)\n  type: oidc-saml-broker\n  operator: tenant\n  host: sso.sydney.edu.au\n  resolves: sydneyuni.customdomains.okta.com\n  detail: >-\n    sso.sydney.edu.au is a vanity hostname CNAMEd to the institution's Okta tenant. It brokers\n    sign-in for\
  \ institution web applications; canvas.sydney.edu.au redirects into it with a\n    SAMLRequest. The contract is Okta's, the tenant is the university's.\n  verified: '2026-08-19'\n- id: session-gated-app-apis\n  name: Session-gated application APIs\n  type: session-cookie\n  operator: institution\n  hosts:\n  - myuni.sydney.edu.au\n  detail: >-\n    The myUni student portal is backed by internal JSON endpoints consumed by the\n    authenticated single-page application. They require an established student session, are\n    not documented, and are not offered to third-party developers.\n  verified: '2026-08-19'\n- id: vendor-issued-api-keys\n  name: Vendor-issued API keys (Ex Libris)\n  type: api-key\n  operator: vendor\n  issuer: https://developers.exlibrisgroup.com/\n  detail: >-\n    Alma and Primo API keys covering the university's library data are issued by Ex Libris to\n    the institution through the Ex Libris Developer Network. The university does not publish or\n    re-issue them.\n\
  maintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sydney/refs/heads/main/authentication/university-of-sydney-authentication.yml
summary_line: 4 schemes
tags:
- University
- Higher Education
- Education
- Australia
- Group of Eight
- Research
- Identity Federation
- Research Repository
- Course Catalog
- Library
---
