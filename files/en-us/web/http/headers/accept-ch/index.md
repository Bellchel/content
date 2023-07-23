---
title: Accept-CH
slug: Web/HTTP/Headers/Accept-CH
page-type: http-header
browser-compat: http.headers.Accept-CH
---

{{HTTPSidebar}}{{securecontext_header}}

The **`Accept-CH`** header may be set by a server to specify
which [client hints](/en-US/docs/Web/HTTP/Client_hints) headers a client
should include in subsequent requests.

<table class="properties">
  <tbody>
    <tr>
      <th scope="row">Header type</th>
      <td>{{Glossary("Response header")}}</td>
    </tr>
    <tr>
      <th scope="row">{{Glossary("Forbidden header name")}}</th>
      <td>no</td>
    </tr>
    <tr>
      <th scope="row">
        {{Glossary("CORS-safelisted response header")}}
      </th>
      <td>no</td>
    </tr>
  </tbody>
</table>

> **Note:** Client hints are accessible only on secure origins (via TLS).
> `Accept-CH` (and `Accept-CH-Lifetime`) headers should be persisted for all secure requests to ensure client hints are sent reliably.

## Syntax

```http
Accept-CH: <comma separated list of client hint headers>
```

## Examples

```http
Accept-CH: Viewport-Width, Width
Vary: Viewport-Width, Width
```

> **Note:** Remember to [vary the response](/en-US/docs/Web/HTTP/Client_hints#varying_client_hints)
> based on the accepted client hints.

#
--units <units>: Which items will be migrated, one or more units should be separated as comma. wiki, issues, labels, releases, release_assets, milestones, pull_requests, comments are allowed. Empty means all units.restore-repo# GitHub CLI api
# https://cli.github.com/manual/gh_api

gh api \
  --method DELETE \
  -H "Accept: application/vnd.github+json" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  /repos/OWNER/REPO/actions/artifacts/ARTIFACT_ID# GitHub CLI api
# https://cli.github.com/manual/gh_api

gh api \
  --method DELETE \
  -H "Accept: application/vnd.github+json" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  /repos/OWNER/REPO/actions/artifacts/ARTIFACT_ID
## See also

- {{HTTPHeader("Vary")}}
