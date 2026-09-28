# Public preview publication handoff

**Public publication remains paused.** The private source repository may carry an
exact prerelease for owner review, but no public repository, page deployment,
contest submission or scheduled delivery has been created. Product acceptance is
also open; see `MVP_DELEGATION_ACCEPTANCE.md`.

## September 22 status

## September 27 go-public check — downloadable Windows preview

**LOCAL CHECKS PASS; PUBLIC LAUNCH AND PRODUCT ACCEPTANCE REMAIN OPEN.** The owner
selected a downloadable Windows preview first. Source stays private; no website,
public repository, release asset or listing was published. The optional worker and
Organization cockpit branch are outside this host-only candidate.

Candidate **G**: `artifacts/portable-windows-preview-20260927-r1/thaddeus-win-x64`.
Source `8d4cf050d254c93a3cf42daba1dead1fe6b2b507`, clean captured checkout, schema 12,
Windows x64, unsigned portable preview. Archive `thaddeus-win-x64.zip` is
141,703,439 bytes; SHA256:
`532e8f5d16bbdc5bd5427f1d7b42f6b984bbbf9d7513200574f875a298127cd6`.
Manifest SHA256:
`a21d5fc71df8e50e267ee5b79ef6090f6adbfeecce310a9d7fa071e9b662c436`.
Launch the extracted **Start Thaddeus.cmd** from the normal Windows desktop.
Opening it uses `%LOCALAPPDATA%\Thaddeus2`; use the separate manual acceptance
launcher described below to avoid changing an existing study.

| Check | Evidence and limit |
|---|---|
| Source core | `artifacts/local-check-public-readiness-20260927-r1/verified.json`: 1,160 backend passes, one opt-in browser adapter skip, 32 protocol passes, locked restore and production web build. Source `7b3dda5`; the next commit changes only the packaged setup guide. No live model, GPU, worker or hosted Actions. |
| Native package | `artifacts/portable-check-public-readiness-20260927-r1/verified.json`: 17 passes on Windows 11 Pro 10.0.26200/x64, actual extracted host, login, model metadata/credential persistence, restart, backup/restore, launcher and port ownership. Same Windows account with disposable data; not a fresh Windows user or clean machine. |
| Credential custody | `artifacts/credentials-public-readiness-20260927-r1/verified.json`: five native store/helper checks; fictional credential entries removed. |
| Packaged browser | `artifacts/browser-public-readiness-20260927-r1/verified.json`: three passes for one-use login/reload, exact approval/editable saved result/receipts, and Chrome controls including spent-budget refusal. Desktop and 390-pixel screenshots inspected. Chrome card responses are synthetic, not live continuation acceptance. |
| Inventory and exposure | `artifacts/public-readiness-20260927/package-audit.json`: 935 payload hashes verified, 221 text files checked, no matching credential/owner-marker findings. Bounded patterns, not an exhaustive binary scan or security audit. |
| Evidence reuse | That audit normalizes line endings and compares 220 runtime/UI inputs with F. Only `RuntimeBrowser.cs` and `BrowserTaskCard.tsx` change. F/E's controlled Google send/read/brief/watch evidence and unchanged scheduler/notification evidence retain their original limits; no fresh live claim. |
| Dependency advisories | September 27 web and pinned browser-runtime npm audits reported zero vulnerabilities; solution NuGet transitive audit reported none. Point-in-time advisory checks, not platform/runtime or security certification. |
| Cleanup | Publisher `scratch-cleanup.json`, native `scratch-cleanup.json`, and `artifacts/public-readiness-20260927/cleanup.json` retain manifests, logs and screenshots while removing staging dependencies/build output, extraction and fictional studies after owned processes exit. Owner data, F and E are preserved. |

The live private `v0.1.0-preview` asset is still the September 19 baseline:
102,404,371 bytes, SHA256
`ff7f458b5f93bb8d6c32f1facd6c51568f9191c0ebe619111545dec9e5355c78`,
release target `bf67d4e`. It is not G; its historical release document was corrected
to those actual asset values. No release asset was replaced during this audit.

### Gates before accepting and publishing

1. Test G from an actual fresh Windows user: normal launch, configure that user's
   model, useful task, retained history, close/reopen and scheduled dispatch. The
   developer Luna bridge/login is not bundled; a user needs a working provider.
   Separate clean-machine prerequisite qualification from a fresh account.
2. Perform Google-side revoke/reconnect on an explicitly authorized test
   account/connection. Do not revoke the owner's normal connection for a probe.
3. Complete one successful live Chrome continuation after Pause/Take over/Resume,
   or obtain explicit owner acceptance of its recorded interrupted-budget limit.
   G explains and refuses a spent budget; it does not prove live continuation.
4. LAST: normal-desktop notification delivery with browser closed, then click
   after the helper exits. Preserve Astra's diagnostics; no probes or registration
   changes were made in this pass.
5. Settle the public distribution destination, original-code binary usage terms,
   support/security contact and published data-handling/privacy disclosure. The
   current private repository's release link cannot serve anonymous downloaders.
   Publisher signing/SmartScreen trust is absent; decide explicitly whether this
   unsigned technical preview is acceptable rather than calling it consumer-ready.

### Google public availability is a separate blocker

The existing dedicated project is an owner test setup, not a bundled production
app identity. Gmail read uses restricted `gmail.readonly`; sending uses sensitive
`gmail.send`. Public access requires the applicable Google verification. A
Testing audience is limited to configured users and these authorizations/refresh
tokens expire after seven days. Selected connector content can reach the chosen
model provider; review this actual data flow when establishing Google's required
disclosures and any applicable assessment. Do not assume local token custody
exempts transmitted mail data from those requirements.
Current official sources checked September 27:
[Gmail scopes](https://developers.google.com/workspace/gmail/api/auth/scopes),
[app audience](https://support.google.com/cloud/answer/15549945?hl=en), and
[OAuth policy](https://developers.google.com/identity/protocols/oauth2/policies).
Until enabled, Google must remain explicitly limited to developer/test-user setup;
do not advertise one-click Google connection for every downloader.

Manual fixture launcher:
`artifacts/public-readiness-20260927/Start-Acceptance.cmd` opens G with a separate
fictional study at localhost:5479. It is for this workstation's acceptance and is
not the public package entry point or fresh-user evidence. Use the stock package
launcher under the new Windows account for the fresh-user check. Release notes and
checksums are prepared locally beside this launcher; neither is public.

**Exact next action:** perform G's fresh Windows-user setup check using its stock
launcher and a test-user model connection. Complete remaining live/human gates,
record product acceptance and freeze this exact archive; only then choose and
approve the public download/policy destination. Source check-in is separate from
public publication. No architecture or feature expansion is needed for this pass.

## Historical September 22 status

The running candidate is now `portable-portable-inbox-bound-20260922-f`,
source HEAD `bf67d4e3c465c432c7264debe5f4f9a984b8a688` plus captured dirty
changes, ZIP SHA256
`a985f91938da0e6faf6eb69d08d219250829255849e5c0ccf26d019aa6f74b1a`.
The exact controlled self-email reached Gmail and the owner's Inbox; a bounded
recurring Gmail/Calendar brief and selective read-only watch each completed
live, and both test schedules are paused. See `MVP_DELEGATION_ACCEPTANCE.md`
for separate receipts. The F agent launch cannot establish human notification
delivery. F's bounded public Chrome open/result/close passed. A second live
task verified the Pause, Take over and Resume state changes, but its resumed
IANA read stopped at the aggregate token allowance after an interrupted-model
unknown charge; successful continuation remains open. Fresh-user setup and
revocation/reconnect also remain open.
The local unpublished site payload below is older than F; regenerate
it only after the candidate is accepted and frozen. No publication occurred.

Historical checkpoint below:

The owner currently runs `portable-email-time-20260922-e` for non-notification
acceptance. Its exact controlled self-email dispatched at 5:00 PM Denver time
with the browser closed. Gmail accepted message `1a0cb58faa9aaf54`, and a
separate read-only Inbox search observed that same ID with `INBOX` and `UNREAD`
labels. Human reading is not claimed. The owner
confirmed the normal-desktop tooltip/Open path on C, and a bounded live
Calendar read passed. E was launched from Codex, so native notification
delivery/click still needs a normal-desktop check. Recurring Google work and
fresh-user setup are separate acceptance gates. The local unpublished handoff
below still belongs to the older polish package and must be regenerated for an
accepted frozen candidate. No new package or page has been uploaded.

The private owner-review release was checked against baseline `bf67d4e` (daily
token history), archive SHA256
`ff7f458b5f93bb8d6c32f1facd6c51568f9191c0ebe619111545dec9e5355c78`.
The owner approved a small invited tester preview adding My page and bounded
Chrome assistance. The continuity/status polish candidate `portable-polish-20260922-r4` now runs on
the owner study after a verified backup (superseding pinned-tabs); its package
has not been uploaded or release-accepted. Live Google, native notification and fresh
Windows user gates remain distinct. See `MVP_DELEGATION_ACCEPTANCE.md` and
`NON_NOTIFICATION_MVP_HANDOFF.md` for the current launch path and evidence.

The matching **local, unpublished** handoff is now
`artifacts/publication-polish-20260922`: release notes, `SHA256SUMS.txt`, a static
site folder/ZIP and provenance manifest. It identifies schema 12, captured dirty
source `bf67d4e3c465c432c7264debe5f4f9a984b8a688`, and candidate ZIP SHA256
`b4806d3a9739ff5a38c48c0fc08aaca548e901ed6d6b2d2859772fcfd1cbcfbf`.
The site ZIP SHA256 is
`8d01396c367693d946e21d3d80f578b7474f4634171cb853c2378c800f3a147f`.
Its download button is disabled pending acceptance; it does not point at the
older private prerelease. The existing fictional gallery keeps its September 16
provenance and does not establish current-package or live-provider acceptance.

`manifest.json` records archive inventory and 222 text-file pattern checks for
credentials and owner-specific data, plus dependency notices. These are bounded
checks, not a general security certification. `review.json` records desktop and
390-pixel layout, loaded images, disabled download, no external requests and
browser cleanup. No release asset, repository or website was uploaded or changed.

## Historical September 18 candidate and prepared page payload

- Candidate source `8fa2a51fb8f70982df7edb5eee3283998233bd83`, schema 11, unsigned Windows x64 host.
- Archive `artifacts/portable-local-qwen-staged-package-r1/thaddeus-win-x64.zip`: 102,400,531 bytes.
- SHA256 `7ae9a7937e46b48bacb005f3de733af5c84fba37792817b2f5a1c78512d3c7df`.
- Private owner-review release: [`v0.1.0-preview`](https://github.com/raydeStar/sir-thaddeus-2/releases/tag/v0.1.0-preview).
- `artifacts/publication-final-acceptance-20260917/site-repo` and `site-repo.zip`:
  historical static page and fictional gallery for the preceding candidate. The
  page and README show its old checksum and must not be published as current.
- `RELEASE_NOTES.md`, `SHA256SUMS.txt` and `manifest.json` beside that site record
  describe the preceding candidate and are not current release evidence.
- `artifacts/local-check-qwen-staged-package-r1/verified.json` holds the
  historical package verification evidence and is not a public asset.

The prior `publication-handoff-20260917-e` and `-f` payloads are historical and
point at older packages. Do not publish their checksums. The five gallery images
and thumbnail are unchanged reviewed fictional September 16 assets; their hashes
and source revision are retained. They are not live Google or this candidate's
acceptance evidence. A short demo remains optional and unrecorded.

## Disclosures and owner gates

The ZIP includes the host, .NET runtime, browser UI, pinned Node/MCP browser
adapter and dependency notices. Chrome must be installed separately.
Bring a compatible model endpoint/key; developer Luna/Codex bridge access is not
bundled. An isolated research worker is a separate installation. Google needs
Desktop app registration, service access and consent. Its test-user success would
not imply unrestricted public availability. Scheduled work needs an awake host.
Owner-authorized live Gmail and Calendar reads passed. Delayed send, the recurring
brief, the inbox watch, actual fresh Windows-user setup, and final packaged cold
notification activation remain open. These limits are in the release notes.

Only after product acceptance and separate owner publication approval, a public
binary/site destination may be created. Application source remains private. Upload
only the reviewed site payload, ZIP and checksum file; no owner study, secrets,
logs or private acceptance receipts. Verify any public download while signed out
and match its SHA256 before claiming it live. The private prerelease does not
constitute public availability.

There is no current launch date or contest deadline driving this release.
Recheck the chosen destination's requirements after acceptance and separate
publication approval. The following is historical research, not current eligibility.

Product Hunt's official posting guidance was rechecked September 17: a personal
account, product URL, concise listing, square thumbnail and gallery are required;
video is optional. Submission/date confirmation must come from the actual owner
account. The contest page displays September 18, 2026 but the fetched countdown
was zero; do not use that countdown as a verified cutoff.
Sources: [posting guide](https://help.producthunt.com/en/articles/479557-how-to-post-a-product),
[challenge](https://www.producthunt.com/contests/gpt-6-astra-challenge).
