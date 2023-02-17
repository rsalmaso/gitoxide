# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 0.4.3 (2023-02-17)

### Bug Fixes

 - <csr-id-e14dc7d475373d2c266e84ff8f1826c68a34ab92/> note that crates have been renamed from `git-*` to `gix-*`.
   This also means that the `git-*` prefixed crates of the `gitoxide` project
   are effectively unmaintained.
   Use the crates with the `gix-*` prefix instead.
   
   If you were using `git-repository`, then `gix` is its substitute.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 1 commit contributed to the release.
 - 7 days passed between releases.
 - 1 commit was understood as [conventional](https://www.conventionalcommits.org).
 - 0 issues like '(#ID)' were seen in commit messages

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **Uncategorized**
    - note that crates have been renamed from `git-*` to `gix-*`. ([`e14dc7d`](https://github.com/Byron/gitoxide/commit/e14dc7d475373d2c266e84ff8f1826c68a34ab92))
</details>

## 0.4.2 (2023-02-09)

### Documentation

 - <csr-id-39ed9eda62b7718d5109135e5ad406fb1fe2978c/> fix typos

### New Features

 - <csr-id-fe04934d783e4c53a79fae2e0d3b0c5802ea1809/> Adds fuzzer for date parser
 - <csr-id-f5c9aa827e3b9ffb82a52ad7f840c58aa0d654ed/> return the time that failed to parse in the error

### Bug Fixes

 - <csr-id-786f6dc5c1f765b9598cd55ca8fb1714ad177e46/> prevent panics from dates which cannot be represented by the `time` crate
 - <csr-id-3d6c81000559df91b17834ec5e9830b085277af8/> panic in `parse_raw()` (as found by fuzzer)

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 17 commits contributed to the release over the course of 28 calendar days.
 - 30 days passed between releases.
 - 5 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 3 unique issues were worked on: [#691](https://github.com/Byron/gitoxide/issues/691), [#711](https://github.com/Byron/gitoxide/issues/711), [#720](https://github.com/Byron/gitoxide/issues/720)

### Thanks Clippy

<csr-read-only-do-not-edit/>

[Clippy](https://github.com/rust-lang/rust-clippy) helped 1 time to make code idiomatic. 

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **[#691](https://github.com/Byron/gitoxide/issues/691)**
    - set `rust-version` to 1.64 ([`55066ce`](https://github.com/Byron/gitoxide/commit/55066ce5fd71209abb5d84da2998b903504584bb))
 * **[#711](https://github.com/Byron/gitoxide/issues/711)**
    - assure we get the latest version of the `time` crate ([`cb31cd1`](https://github.com/Byron/gitoxide/commit/cb31cd16bc4a6e749c298cfbc7e0dad05b11b96c))
 * **[#720](https://github.com/Byron/gitoxide/issues/720)**
    - prevent panics from dates which cannot be represented by the `time` crate ([`786f6dc`](https://github.com/Byron/gitoxide/commit/786f6dc5c1f765b9598cd55ca8fb1714ad177e46))
 * **Uncategorized**
    - Release git-date v0.4.2, git-hash v0.10.2, git-features v0.26.2, git-actor v0.17.1, git-glob v0.5.3, git-path v0.7.1, git-quote v0.4.1, git-attributes v0.8.2, git-config-value v0.10.1, git-tempfile v3.0.2, git-lock v3.0.2, git-validate v0.7.2, git-object v0.26.1, git-ref v0.24.0, git-sec v0.6.2, git-config v0.16.0, git-command v0.2.3, git-prompt v0.3.2, git-url v0.13.2, git-credentials v0.9.1, git-diff v0.26.1, git-discover v0.13.0, git-hashtable v0.1.1, git-bitmap v0.2.1, git-traverse v0.22.1, git-index v0.12.3, git-mailmap v0.9.2, git-chunk v0.4.1, git-pack v0.30.2, git-odb v0.40.2, git-packetline v0.14.2, git-transport v0.25.4, git-protocol v0.26.3, git-revision v0.10.2, git-refspec v0.7.2, git-worktree v0.12.2, git-repository v0.34.0, safety bump 3 crates ([`c196d20`](https://github.com/Byron/gitoxide/commit/c196d206d57a310b1ce974a1cf0e7e6d6db5c4d6))
    - prepare changelogs prior to release ([`7c846d2`](https://github.com/Byron/gitoxide/commit/7c846d2102dc767366771925212712ef8cc9bf07))
    - Merge branch 'Lioness100/main' ([`1e544e8`](https://github.com/Byron/gitoxide/commit/1e544e82455bf9ecb5e3c2146280eaf7ecd81f16))
    - fix typos ([`39ed9ed`](https://github.com/Byron/gitoxide/commit/39ed9eda62b7718d5109135e5ad406fb1fe2978c))
    - thanks clippy ([`bac57dd`](https://github.com/Byron/gitoxide/commit/bac57dd05ea2d5a4ee45ef9350fa3f2e19474bc0))
    - Merge branch 'adjustments-for-cargo' ([`7bba270`](https://github.com/Byron/gitoxide/commit/7bba2709488b7eb999b8136dbab03af977241678))
    - Merge branch 'fix-gix-date-panics' ([`56f5593`](https://github.com/Byron/gitoxide/commit/56f5593b25e300d21c380c5fb5a184445ff26183))
    - panic in `parse_raw()` (as found by fuzzer) ([`3d6c810`](https://github.com/Byron/gitoxide/commit/3d6c81000559df91b17834ec5e9830b085277af8))
    - fix warnings, don't track Cargo.lock to use compatible latest dependencies ([`96a56a9`](https://github.com/Byron/gitoxide/commit/96a56a9d1d76e5832a4bf505152985a74c6c7357))
    - Merge pull request #714 from silvergasp/fuzz-gix-date ([`a52c54e`](https://github.com/Byron/gitoxide/commit/a52c54e97698c1b61ff70884378338f63b4d1a27))
    - Adds fuzzer for date parser ([`fe04934`](https://github.com/Byron/gitoxide/commit/fe04934d783e4c53a79fae2e0d3b0c5802ea1809))
    - Optimize usage of `hex_to_id()` ([`6fa950d`](https://github.com/Byron/gitoxide/commit/6fa950d0ab1991a5577c06385169be1b390dd88a))
    - Break cyclical dev dependencies ([`1fea18f`](https://github.com/Byron/gitoxide/commit/1fea18f5f8b4189a23dc4fa3f041a672f6fbcfb3))
    - return the time that failed to parse in the error ([`f5c9aa8`](https://github.com/Byron/gitoxide/commit/f5c9aa827e3b9ffb82a52ad7f840c58aa0d654ed))
</details>

## 0.4.1 (2023-01-10)

A maintenance release without user-facing changes.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 4 commits contributed to the release.
 - 3 days passed between releases.
 - 0 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 0 issues like '(#ID)' were seen in commit messages

### Thanks Clippy

<csr-read-only-do-not-edit/>

[Clippy](https://github.com/rust-lang/rust-clippy) helped 1 time to make code idiomatic. 

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **Uncategorized**
    - Release gix-date v0.4.1, gix-features v0.26.1, gix-glob v0.5.2, gix-attributes v0.8.1, gix-tempfile v3.0.1, gix-ref v0.23.1, gix-sec v0.6.1, gix-config v0.15.1, gix-prompt v0.3.1, gix-url v0.13.1, gix-discover v0.12.1, gix-index v0.12.2, gix-mailmap v0.9.1, gix-pack v0.30.1, gix-odb v0.40.1, gix-transport v0.25.3, gix-protocol v0.26.2, gix-revision v0.10.1, gix-refspec v0.7.1, gix-worktree v0.12.1, git-repository v0.33.0 ([`5b5b380`](https://github.com/Byron/gitoxide/commit/5b5b3809faa71c658db38b40dfc410224d08a367))
    - prepare changelogs prior to release ([`93bef97`](https://github.com/Byron/gitoxide/commit/93bef97b3c0c75d4bf7119fdd787516e1efc77bf))
    - Merge branch 'patch-1' ([`b93f0c4`](https://github.com/Byron/gitoxide/commit/b93f0c49fc677b6c19aea332cbfc1445ce475375))
    - thanks clippy ([`b34c9fe`](https://github.com/Byron/gitoxide/commit/b34c9fe58223862712eacc1cb7353e497a4b9778))
</details>

## 0.4.0 (2023-01-06)

<csr-id-41fc2bb20e6a926ffc3638c0fac21d733fdc2e3c/>

### New Features

 - <csr-id-4066ac7367d8e870522746429513fb7a357a2cc6/> Support git default date format
   This is the format output by default by `git log` or when using
   `--pretty=%ad`.
   
   The new gix_date::time::format::GIT_DEFAULT format description may be used
   to output date strings in this format. It is also now used by
   gix_date::parse() to accept date strings that may be in this format.
 - <csr-id-8094351fe547a0f6756b0ed29dc87a0e6b9ceec1/> Format git-style RFC 2822 date strings
   Git outputs the day-of-month field as a non-padded number whereas strict
   RFC 2822 date strings are supposed to use a zero-padded two-digit number.
   
   The new gix_date::time::format::GIT_RFC2822 format description allows Time
   to be formatted in git's RFC 2822 style. (Whereas the existing RFC2822
   format description produces a strict RFC 2822 date string).

### Bug Fixes

<csr-id-dff0aa0be600b9cd9518184fefa9b3c8fdb510f2/>

 - <csr-id-046af94f005a6e095f0d3616c0b57ef1f556f734/> Stricter raw date parsing
   The raw date parser (gix_date::parse::function::parse_raw()) accepted some
   inputs that it should not have. Specifically, it would accept:
   
   - Any character for the timezone offset's sign

### Other (BREAKING)

 - <csr-id-41fc2bb20e6a926ffc3638c0fac21d733fdc2e3c/> `time::format::GIT_DEFAULT` -> `*::DEFAULT` and `*::DEFAULT` -> `*::GITOXIDE`.
   That way we properly indicate what we are doing and don't try to somewhat
   sneakily suggest that the default for git dates is something else
   due to personal preference.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 10 commits contributed to the release over the course of 6 calendar days.
 - 18 days passed between releases.
 - 5 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 0 issues like '(#ID)' were seen in commit messages

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **Uncategorized**
    - Release gix-date v0.4.0, gix-actor v0.17.0, gix-object v0.26.0, gix-traverse v0.22.0, gix-index v0.12.0, safety bump 15 crates ([`0e3d0a5`](https://github.com/Byron/gitoxide/commit/0e3d0a56d7e6a60c6578138f2690b4fa54a2072d))
    - prepare changelogs prior to release ([`d679f5b`](https://github.com/Byron/gitoxide/commit/d679f5b6f018633e858d3ebbdaf1cd5098bbc5e7))
    - `time::format::GIT_DEFAULT` -> `*::DEFAULT` and `*::DEFAULT` -> `*::GITOXIDE`. ([`41fc2bb`](https://github.com/Byron/gitoxide/commit/41fc2bb20e6a926ffc3638c0fac21d733fdc2e3c))
    - Merge branch 'strict-raw-dates' ([`c65ce7e`](https://github.com/Byron/gitoxide/commit/c65ce7e3031b036d3a76b6e8a6c9ead39390261c))
    - Stricter raw date parsing ([`046af94`](https://github.com/Byron/gitoxide/commit/046af94f005a6e095f0d3616c0b57ef1f556f734))
    - Merge branch 'issue-679' ([`a910d9e`](https://github.com/Byron/gitoxide/commit/a910d9e7dcb2ba1979660165fa5b8cb0a2dce594))
    - refactor ([`26597b9`](https://github.com/Byron/gitoxide/commit/26597b983d401a1efcd13b3e69aad6a39581ec0b))
    - Support git default date format ([`4066ac7`](https://github.com/Byron/gitoxide/commit/4066ac7367d8e870522746429513fb7a357a2cc6))
    - Format git-style RFC 2822 date strings ([`8094351`](https://github.com/Byron/gitoxide/commit/8094351fe547a0f6756b0ed29dc87a0e6b9ceec1))
    - Parse git-styled RFC 2822 date strings ([`dff0aa0`](https://github.com/Byron/gitoxide/commit/dff0aa0be600b9cd9518184fefa9b3c8fdb510f2))
</details>

## 0.3.1 (2022-12-19)

### Bug Fixes

 - <csr-id-39655f5f6fa39a55c4420f672e866c483f9b85ed/> Negative system timezone offsets should be serialized as such
 - <csr-id-f4ea59db0a429801ab40b1294da4bffd9e0f80b3/> correctly parse raw dates with negative timezone offsets
 - <csr-id-be603f593055309b74685bc2aebb8e35e6de2d59/> always consider timestamps as UTC when loading from commits

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 16 commits contributed to the release over the course of 27 calendar days.
 - 27 days passed between releases.
 - 3 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 0 issues like '(#ID)' were seen in commit messages

### Thanks Clippy

<csr-read-only-do-not-edit/>

[Clippy](https://github.com/rust-lang/rust-clippy) helped 1 time to make code idiomatic. 

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **Uncategorized**
    - Release gix-date v0.3.1, gix-features v0.25.0, gix-actor v0.15.0, gix-glob v0.5.1, gix-path v0.7.0, gix-attributes v0.7.0, gix-config-value v0.10.0, gix-lock v3.0.1, gix-validate v0.7.1, gix-object v0.24.0, gix-ref v0.21.0, gix-sec v0.6.0, gix-config v0.13.0, gix-prompt v0.3.0, gix-url v0.12.0, gix-credentials v0.8.0, gix-diff v0.24.0, gix-discover v0.10.0, gix-traverse v0.20.0, gix-index v0.10.0, gix-mailmap v0.7.0, gix-pack v0.28.0, gix-odb v0.38.0, gix-packetline v0.14.1, gix-transport v0.24.0, gix-protocol v0.25.0, gix-revision v0.8.0, gix-refspec v0.5.0, gix-worktree v0.10.0, git-repository v0.30.0, safety bump 26 crates ([`e6b9906`](https://github.com/Byron/gitoxide/commit/e6b9906c486b11057936da16ed6e0ec450a0fb83))
    - prepare chnagelogs prior to git-repository release ([`7114bbb`](https://github.com/Byron/gitoxide/commit/7114bbb6732aa8571d4ab74f28ed3e26e9fbe4d0))
    - Merge branch 'main' into read-split-index ([`c57bdde`](https://github.com/Byron/gitoxide/commit/c57bdde6de37eca9672ea715962bbd02aa3eb055))
    - Merge branch 'adjustments-for-cargo' ([`083909b`](https://github.com/Byron/gitoxide/commit/083909bc7eb902eeee2002034fdb6ed88280dc5c))
    - Merge branch 'bugfix/system-time-correct-offset-sign' ([`6e40433`](https://github.com/Byron/gitoxide/commit/6e40433f6f607888e8f8a6c36e53a68b91fcf671))
    - Add non-isolated test that, depending on region, would catch the invalid-sign bug. ([`b649965`](https://github.com/Byron/gitoxide/commit/b6499653b71e79f17a7304c6e83d2e1776ff5d5e))
    - Negative system timezone offsets should be serialized as such ([`39655f5`](https://github.com/Byron/gitoxide/commit/39655f5f6fa39a55c4420f672e866c483f9b85ed))
    - adjust to changes in `gix-testtools` ([`4eb842c`](https://github.com/Byron/gitoxide/commit/4eb842c7150b980e1c2637217e1f9657a671cea7))
    - Merge branch 'bugfix/signed-raw-time' ([`f50b9f5`](https://github.com/Byron/gitoxide/commit/f50b9f54425e64461a31d00e082470aa5042be74))
    - thanks clippy ([`75d6e88`](https://github.com/Byron/gitoxide/commit/75d6e882cea823100f2ad5bf26a4f1082287d80b))
    - refactor ([`f4e8051`](https://github.com/Byron/gitoxide/commit/f4e8051fbc8cde9ba25fb1185c9e32f6aed4c0fb))
    - correctly parse raw dates with negative timezone offsets ([`f4ea59d`](https://github.com/Byron/gitoxide/commit/f4ea59db0a429801ab40b1294da4bffd9e0f80b3))
    - Extend gix-date's baseline tests to also re-format the parsed dates ([`9f95f7f`](https://github.com/Byron/gitoxide/commit/9f95f7fbbe5b56e65c00c26f580bf67a4001e146))
    - Merge branch 'bugfix/timestamp-to-datetime-conversion' ([`be0bbf5`](https://github.com/Byron/gitoxide/commit/be0bbf519c4a6687c305717ec0c12215a5836f58))
    - always consider timestamps as UTC when loading from commits ([`be603f5`](https://github.com/Byron/gitoxide/commit/be603f593055309b74685bc2aebb8e35e6de2d59))
    - Merge branch 'main' into http-config ([`bcd9654`](https://github.com/Byron/gitoxide/commit/bcd9654e56169799eb706646da6ee1f4ef2021a9))
</details>

## 0.3.0 (2022-11-21)

### New Features (BREAKING)

 - <csr-id-3d8fa8fef9800b1576beab8a5bc39b821157a5ed/> upgrade edition to 2021 in most crates.
   MSRV for this is 1.56, and we are now at 1.60 so should be compatible.
   This isn't more than a patch release as it should break nobody
   who is adhering to the MSRV, but let's be careful and mark it
   breaking.
   
   Note that `gix-features` and `gix-pack` are still on edition 2018
   as they make use of a workaround to support (safe) mutable access
   to non-overlapping entries in a slice which doesn't work anymore
   in edition 2021.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 5 commits contributed to the release over the course of 62 calendar days.
 - 62 days passed between releases.
 - 1 commit was understood as [conventional](https://www.conventionalcommits.org).
 - 0 issues like '(#ID)' were seen in commit messages

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **Uncategorized**
    - Release gix-hash v0.10.0, gix-features v0.24.0, gix-date v0.3.0, gix-actor v0.14.0, gix-glob v0.5.0, gix-path v0.6.0, gix-quote v0.4.0, gix-attributes v0.6.0, gix-config-value v0.9.0, gix-tempfile v3.0.0, gix-lock v3.0.0, gix-validate v0.7.0, gix-object v0.23.0, gix-ref v0.20.0, gix-sec v0.5.0, gix-config v0.12.0, gix-command v0.2.0, gix-prompt v0.2.0, gix-url v0.11.0, gix-credentials v0.7.0, gix-diff v0.23.0, gix-discover v0.9.0, gix-bitmap v0.2.0, gix-traverse v0.19.0, gix-index v0.9.0, gix-mailmap v0.6.0, gix-chunk v0.4.0, gix-pack v0.27.0, gix-odb v0.37.0, gix-packetline v0.14.0, gix-transport v0.23.0, gix-protocol v0.24.0, gix-revision v0.7.0, gix-refspec v0.4.0, gix-worktree v0.9.0, git-repository v0.29.0, gix-commitgraph v0.11.0, gitoxide-core v0.21.0, gitoxide v0.19.0, safety bump 28 crates ([`b2c301e`](https://github.com/Byron/gitoxide/commit/b2c301ef131ffe1871314e19f387cf10a8d2ac16))
    - prepare changelogs prior to release ([`e4648f8`](https://github.com/Byron/gitoxide/commit/e4648f827c97e9d13636d1bbdc83dd63436e6e5c))
    - Merge branch 'version2021' ([`0e4462d`](https://github.com/Byron/gitoxide/commit/0e4462df7a5166fe85c23a779462cdca8ee013e8))
    - upgrade edition to 2021 in most crates. ([`3d8fa8f`](https://github.com/Byron/gitoxide/commit/3d8fa8fef9800b1576beab8a5bc39b821157a5ed))
    - Merge branch 'diff' ([`25a7726`](https://github.com/Byron/gitoxide/commit/25a7726377fbe400ea3c4927d04e9dec99802b7b))
</details>

## 0.2.0 (2022-09-20)

### Changed (BREAKING)

 - <csr-id-99905bacace8aed42b16d43f0f04cae996cb971c/> upgrade `bstr` to `1.0.1`
 - <csr-id-c24ea67f84aa48953949682672114715bee67432/> parse now takes the current time `parse(…, Option<time>)` as parameter.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 34 commits contributed to the release over the course of 27 calendar days.
 - 27 days passed between releases.
 - 2 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 2 unique issues were worked on: [#450](https://github.com/Byron/gitoxide/issues/450), [#470](https://github.com/Byron/gitoxide/issues/470)

### Thanks Clippy

<csr-read-only-do-not-edit/>

[Clippy](https://github.com/rust-lang/rust-clippy) helped 1 time to make code idiomatic. 

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **[#450](https://github.com/Byron/gitoxide/issues/450)**
    - upgrade `bstr` to `1.0.1` ([`99905ba`](https://github.com/Byron/gitoxide/commit/99905bacace8aed42b16d43f0f04cae996cb971c))
 * **[#470](https://github.com/Byron/gitoxide/issues/470)**
    - update changelogs prior to release ([`caa7a1b`](https://github.com/Byron/gitoxide/commit/caa7a1bdef74d7d3166a7e38127a59f5ab3cfbdd))
 * **Uncategorized**
    - Release gix-hash v0.9.10, gix-features v0.22.5, gix-date v0.2.0, gix-actor v0.12.0, gix-glob v0.4.0, gix-path v0.5.0, gix-quote v0.3.0, gix-attributes v0.4.0, gix-config-value v0.8.0, gix-tempfile v2.0.5, gix-validate v0.6.0, gix-object v0.21.0, gix-ref v0.16.0, gix-sec v0.4.0, gix-config v0.8.0, gix-discover v0.5.0, gix-traverse v0.17.0, gix-index v0.5.0, gix-worktree v0.5.0, gix-testtools v0.9.0, gix-command v0.1.0, gix-prompt v0.1.0, gix-url v0.9.0, gix-credentials v0.5.0, gix-diff v0.19.0, gix-mailmap v0.4.0, gix-chunk v0.3.2, gix-pack v0.23.0, gix-odb v0.33.0, gix-packetline v0.13.0, gix-transport v0.20.0, gix-protocol v0.20.0, gix-revision v0.5.0, gix-refspec v0.2.0, git-repository v0.24.0, gix-commitgraph v0.9.0, gitoxide-core v0.18.0, gitoxide v0.16.0, safety bump 28 crates ([`29a043b`](https://github.com/Byron/gitoxide/commit/29a043be6808a3e9199a9b26bd076fe843afe4f4))
    - Merge branch 'filter-refs' ([`fd14489`](https://github.com/Byron/gitoxide/commit/fd14489f729172d615d0fa1e8dbd605e9eacf69d))
    - Merge branch 'git_date_relative' ([`83a3832`](https://github.com/Byron/gitoxide/commit/83a38329c59e9ebc057221da832fd8320bbeddb1))
    - refactor ([`c5c6bf6`](https://github.com/Byron/gitoxide/commit/c5c6bf6ef3f0c9c12389bb638ab4d32b61839dec))
    - refactor ([`956613f`](https://github.com/Byron/gitoxide/commit/956613fcdb33a845526fa9743aa0e7f80b3badfa))
    - refactor ([`1026b7c`](https://github.com/Byron/gitoxide/commit/1026b7c613a3a8b46a27dd7cd5e3520043b21ab7))
    - WIP. ([`79d82d4`](https://github.com/Byron/gitoxide/commit/79d82d46613c83280d2401ef4d72a35010a70b87))
    - Parse the output while parsing the baseline file. ([`70fe59f`](https://github.com/Byron/gitoxide/commit/70fe59f4a1cad25f687397206ee2cbe50e643181))
    - make fmt ([`535e967`](https://github.com/Byron/gitoxide/commit/535e967666c6da657ff1b7eff7c64ab27cafb182))
    - Merge branch 'main' into filter-refs-by-spec ([`1f6e5ab`](https://github.com/Byron/gitoxide/commit/1f6e5ab15f5fd8d23719b13e6aea59cd231ac0fe))
    - parse now takes the current time `parse(…, Option<time>)` as parameter. ([`c24ea67`](https://github.com/Byron/gitoxide/commit/c24ea67f84aa48953949682672114715bee67432))
    - Merge branch 'git_date_parse' ([`75591fb`](https://github.com/Byron/gitoxide/commit/75591fb108ce440ba2f920bebf99158b407e3046))
    - thanks clippy ([`590fcc9`](https://github.com/Byron/gitoxide/commit/590fcc9f3fc768802fd09f4e73036e225ec5c363))
    - a sample on how to more easily test relative date parsing ([`c585c9b`](https://github.com/Byron/gitoxide/commit/c585c9b2b0e628914169bbfba55aa5130da51a83))
    - add test to check times before unix epoch ([`eb304ea`](https://github.com/Byron/gitoxide/commit/eb304ea91f857070380ef4e4dbdff6b8ab89cee1))
    - refactor ([`0e231eb`](https://github.com/Byron/gitoxide/commit/0e231ebeeb41306b1075bc06c78b45dc65ded5fa))
    - refactor ([`5793465`](https://github.com/Byron/gitoxide/commit/5793465b0f19b284a4615290e2b08203e969e9bb))
    - refactor; add failing test to see invalid date error in action ([`90008aa`](https://github.com/Byron/gitoxide/commit/90008aa4e59f78cfe2ecd5a7ee851bb56f7b0d33))
    - Merge branch 'main' into index-from-tree ([`bc64b96`](https://github.com/Byron/gitoxide/commit/bc64b96a2ec781c72d1d4daad38aa7fb8b74f99b))
    - PR comments. ([`1eac4de`](https://github.com/Byron/gitoxide/commit/1eac4de99de250e770b48054fd5bc6b806418e4d))
    - `parse` is pure function. ([`9ad1a5f`](https://github.com/Byron/gitoxide/commit/9ad1a5fa2ce54e978396ff3eaa7061a8edd10d4a))
    - Fallible timestamp cast i64 -> u32. ([`cce7616`](https://github.com/Byron/gitoxide/commit/cce7616835f1dff29b2c74bd96b5238d55167d5f))
    - `parse()` returns Result. ([`206f392`](https://github.com/Byron/gitoxide/commit/206f3923f5da2e9e26677e917550e6e5baa2913a))
    - Add output to baseline. ([`5c3b733`](https://github.com/Byron/gitoxide/commit/5c3b7334289ef71a9dbcc021f1989eb8e021fc7f))
    - `parse` returns Result. ([`67c8c6a`](https://github.com/Byron/gitoxide/commit/67c8c6a9666161a3a0cd01203e0fb1da22336939))
    - Add fixtures. ([`6c40ac1`](https://github.com/Byron/gitoxide/commit/6c40ac1e39fbefba640fc9cb4fd3ef419a149e99))
    - Add git baseline. ([`b747a60`](https://github.com/Byron/gitoxide/commit/b747a60b62c533b3919124e628f31e6bbef9c838))
    - refactor ([`3e6e0f9`](https://github.com/Byron/gitoxide/commit/3e6e0f9ebdf7ab87c689be074ae1eecfea4485f0))
    - Draft. ([`95b4902`](https://github.com/Byron/gitoxide/commit/95b490230ebfbd4c2f04edd7074d5a0f5e2429ec))
    - Draft. ([`43b6c06`](https://github.com/Byron/gitoxide/commit/43b6c064bfa407d1a2cabf09aad1cc8334dec651))
    - Merge branch 'main' into filter-refs-by-spec ([`cfa1440`](https://github.com/Byron/gitoxide/commit/cfa144031dbcac2707ab0cec012bc35e78f9c475))
    - Merge branch 'fix-ci-installation' ([`9245083`](https://github.com/Byron/gitoxide/commit/92450839621a4d99cb22d08cbf9f9a89ff6b9e3f))
</details>

## 0.1.0 (2022-08-24)

### New Features

 - <csr-id-034c8dc4437c06dc8af702fbe9b86ec903c73a18/> bump version to 1.0 to prevent accidental inclusions downstream
   For some reason, cargo considers different patch releases breaking, so
   creating a new patch can break installation of gitoxide entirely.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 3 commits contributed to the release.
 - 1 commit was understood as [conventional](https://www.conventionalcommits.org).
 - 0 issues like '(#ID)' were seen in commit messages

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **Uncategorized**
    - Release gix-date v0.1.0, gix-actor v0.11.4, gix-revision v0.4.3, git-repository v0.22.1, cargo-smart-release v0.11.0, gix-commitgraph v0.8.2, gitoxide-core v0.17.0, gitoxide v0.15.0 ([`1fb931a`](https://github.com/Byron/gitoxide/commit/1fb931a7ea59f1cf895a6c1392fd8615b723c743))
    - update changelogs prior to release ([`23cb58f`](https://github.com/Byron/gitoxide/commit/23cb58f02043e0e5027136fd6e8e724c03a2efbe))
    - bump version to 1.0 to prevent accidental inclusions downstream ([`034c8dc`](https://github.com/Byron/gitoxide/commit/034c8dc4437c06dc8af702fbe9b86ec903c73a18))
</details>

## 0.0.5 (2022-08-24)

<csr-id-f7f136dbe4f86e7dee1d54835c420ec07c96cd78/>
<csr-id-533e887e80c5f7ede8392884562e1c5ba56fb9a8/>

### Chore

 - <csr-id-f7f136dbe4f86e7dee1d54835c420ec07c96cd78/> uniformize deny attributes
 - <csr-id-533e887e80c5f7ede8392884562e1c5ba56fb9a8/> remove default link to cargo doc everywhere

### New Features

 - <csr-id-b1c40b0364ef092cd52d03b34f491b254816b18d/> use docsrs feature in code to show what is feature-gated automatically on docs.rs
 - <csr-id-517677147f1c17304c62cf97a1dd09f232ebf5db/> pass --cfg docsrs when compiling for https://docs.rs

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 10 commits contributed to the release over the course of 4 calendar days.
 - 4 days passed between releases.
 - 4 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 0 issues like '(#ID)' were seen in commit messages

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **Uncategorized**
    - Release gix-date v0.0.5, gix-hash v0.9.8, gix-features v0.22.2, gix-actor v0.11.3, gix-glob v0.3.2, gix-quote v0.2.1, gix-attributes v0.3.2, gix-tempfile v2.0.4, gix-lock v2.1.1, gix-validate v0.5.5, gix-object v0.20.2, gix-ref v0.15.2, gix-sec v0.3.1, gix-config v0.7.0, gix-credentials v0.4.0, gix-diff v0.17.2, gix-discover v0.4.1, gix-bitmap v0.1.2, gix-index v0.4.2, gix-mailmap v0.3.2, gix-chunk v0.3.1, gix-traverse v0.16.2, gix-pack v0.21.2, gix-odb v0.31.2, gix-packetline v0.12.7, gix-url v0.7.2, gix-transport v0.19.2, gix-protocol v0.19.0, gix-revision v0.4.2, gix-refspec v0.1.0, gix-worktree v0.4.2, git-repository v0.22.0, safety bump 4 crates ([`4974eca`](https://github.com/Byron/gitoxide/commit/4974eca96d525d1ee4f8cad79bb713af7a18bf9d))
    - Merge pull request #497 from svetli-n/patch-2 ([`bd02b39`](https://github.com/Byron/gitoxide/commit/bd02b392734d8074adedc504a2cf69952d6fa980))
    - Fix doc comment ([`51cd9ce`](https://github.com/Byron/gitoxide/commit/51cd9ceda6a8a0127a18802dc2cc49861013a65d))
    - Merge branch 'main' into remote-ls-refs ([`e2ee3de`](https://github.com/Byron/gitoxide/commit/e2ee3ded97e5c449933712883535b30d151c7c78))
    - Merge branch 'docsrs-show-features' ([`31c2351`](https://github.com/Byron/gitoxide/commit/31c235140cad212d16a56195763fbddd971d87ce))
    - use docsrs feature in code to show what is feature-gated automatically on docs.rs ([`b1c40b0`](https://github.com/Byron/gitoxide/commit/b1c40b0364ef092cd52d03b34f491b254816b18d))
    - uniformize deny attributes ([`f7f136d`](https://github.com/Byron/gitoxide/commit/f7f136dbe4f86e7dee1d54835c420ec07c96cd78))
    - pass --cfg docsrs when compiling for https://docs.rs ([`5176771`](https://github.com/Byron/gitoxide/commit/517677147f1c17304c62cf97a1dd09f232ebf5db))
    - remove default link to cargo doc everywhere ([`533e887`](https://github.com/Byron/gitoxide/commit/533e887e80c5f7ede8392884562e1c5ba56fb9a8))
    - Merge branch 'main' into remote-ls-refs ([`c82bbfa`](https://github.com/Byron/gitoxide/commit/c82bbfaddc45bf9b5b55f056613046d977d9ef09))
</details>

## 0.0.4 (2022-08-19)

### New Features

 - <csr-id-8f7f9ce2b06ec884220b8cd5010b3df04b1ff0bc/> Raw and Unix formats.
 - <csr-id-4b0c2198f9d5b28584c717123c7cfb1b27724605/> Add ISO-strict format

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 10 commits contributed to the release.
 - 1 day passed between releases.
 - 2 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 0 issues like '(#ID)' were seen in commit messages

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **Uncategorized**
    - Release gix-date v0.0.4, gix-actor v0.11.2, gix-revision v0.4.1, git-repository v0.21.1 ([`2f9dc84`](https://github.com/Byron/gitoxide/commit/2f9dc847e0d54f4181ce35ddadd9286ba80ca01f))
    - update changelogs prior to release ([`1b5fd86`](https://github.com/Byron/gitoxide/commit/1b5fd86d121634f8567e8442f125377e460032c6))
    - prepare for release of git-repository ([`8aa5389`](https://github.com/Byron/gitoxide/commit/8aa5389d5a1bdd3a07f1caa1c2f55c8af4f9844a))
    - Merge branch 'add_common_git_formats' ([`c53e5a4`](https://github.com/Byron/gitoxide/commit/c53e5a4c521fbae7d74ad8323f79ced4dfe4f037))
    - Raw and Unix formats. ([`8f7f9ce`](https://github.com/Byron/gitoxide/commit/8f7f9ce2b06ec884220b8cd5010b3df04b1ff0bc))
    - Foundation for custom formats that aren't easily done with `time` formatting ([`b74eaf8`](https://github.com/Byron/gitoxide/commit/b74eaf85d41e1ec67d8c84cc8484702514c3e7cd))
    - Add ISO-strict format ([`4b0c219`](https://github.com/Byron/gitoxide/commit/4b0c2198f9d5b28584c717123c7cfb1b27724605))
    - refinements ([`b1fea0f`](https://github.com/Byron/gitoxide/commit/b1fea0fe76bd94850c7da34ee9504525ad667748))
    - Add common git date formats. ([`090795b`](https://github.com/Byron/gitoxide/commit/090795b4040e2dad995390e502f87c2ced8045f8))
    - Merge branch 'main' into remote-ls-refs ([`bd5f3e8`](https://github.com/Byron/gitoxide/commit/bd5f3e8db7e0bb4abfb7b0f79f585ab82c3a14ab))
</details>

## 0.0.3 (2022-08-17)

A maintenance release without user facing changes.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 21 commits contributed to the release over the course of 25 calendar days.
 - 26 days passed between releases.
 - 0 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 1 unique issue was worked on: [#427](https://github.com/Byron/gitoxide/issues/427)

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **[#427](https://github.com/Byron/gitoxide/issues/427)**
    - make fmt ([`4b320e7`](https://github.com/Byron/gitoxide/commit/4b320e773368ac5e8c38dd8a779ef3d6d2d024ec))
    - git-style disambiguation errors ([`5717194`](https://github.com/Byron/gitoxide/commit/57171946081c03da98f3d33f5b963c3bc4b2d6d9))
 * **Uncategorized**
    - Release gix-date v0.0.3, gix-actor v0.11.1, gix-attributes v0.3.1, gix-tempfile v2.0.3, gix-object v0.20.1, gix-ref v0.15.1, gix-config v0.6.1, gix-diff v0.17.1, gix-discover v0.4.0, gix-bitmap v0.1.1, gix-index v0.4.1, gix-mailmap v0.3.1, gix-traverse v0.16.1, gix-pack v0.21.1, gix-odb v0.31.1, gix-packetline v0.12.6, gix-url v0.7.1, gix-transport v0.19.1, gix-protocol v0.18.1, gix-revision v0.4.0, gix-worktree v0.4.1, git-repository v0.21.0, safety bump 5 crates ([`c96473d`](https://github.com/Byron/gitoxide/commit/c96473dce21c3464aacbc0a62d520c1a33172611))
    - prepare changelogs prior to reelase ([`c06ae1c`](https://github.com/Byron/gitoxide/commit/c06ae1c606b6af9c2a12021103d99c2810750d60))
    - Merge branch 'main' into remote-ls-refs ([`c4bf958`](https://github.com/Byron/gitoxide/commit/c4bf9585d815bc342e5fb383336cc654280dd34f))
    - adjust `gix_date::parsea(str)` to use a str ([`0f8680a`](https://github.com/Byron/gitoxide/commit/0f8680a60913556b7fbd7543fda6a409ac05b121))
    - refactor ([`11a5fa2`](https://github.com/Byron/gitoxide/commit/11a5fa29615d47c24f78446a1c3f5d3b8acf2f93))
    - refactor ([`8e6f4a9`](https://github.com/Byron/gitoxide/commit/8e6f4a921b6b45945e711aaf5858b7714371fb41))
    - Merge branch 'format_git_date_time' ([`99e12be`](https://github.com/Byron/gitoxide/commit/99e12bee16ab3f344c71818bfd1c95cf50e1721b))
    - thanks clipppy ([`b139d70`](https://github.com/Byron/gitoxide/commit/b139d7043fbbbe5b933d96e83544059fe2a7bdd8))
    - refactor ([`bd64387`](https://github.com/Byron/gitoxide/commit/bd64387d8ad3377571755dff14577cc3c53ee9cc))
    - Use time format strings. ([`f84e8f5`](https://github.com/Byron/gitoxide/commit/f84e8f5f16ec2197d1967fb1cc06e9609ea52c16))
    - refactor ([`556dd8c`](https://github.com/Byron/gitoxide/commit/556dd8cb78ea9321031984e2c6b4f9bc415f1be5))
    - refactor ([`5bbcbcd`](https://github.com/Byron/gitoxide/commit/5bbcbcd75d1ab26746da7a927390ff3b6cc19a85))
    - Format `gix-date::Time` with `time::format_description`. ([`d4243bc`](https://github.com/Byron/gitoxide/commit/d4243bc4feb994bde99156ba77fff63bc9c875e9))
    - Merge branch 'rev-parse-delegate' ([`2f506c7`](https://github.com/Byron/gitoxide/commit/2f506c7c2988477b0f97d272a9ac9ed47b236457))
    - Merge pull request #2 from SidneyDouw/main ([`ce885ad`](https://github.com/Byron/gitoxide/commit/ce885ad4c3324c09c83751c32e014f246c748766))
    - Merge branch 'Byron:main' into main ([`9b9ea02`](https://github.com/Byron/gitoxide/commit/9b9ea0275f8ff5862f24cf5a4ca53bb1cd610709))
    - Merge branch 'main' into rev-parse-delegate ([`6da8250`](https://github.com/Byron/gitoxide/commit/6da82507588d3bc849217c11d9a1d398b67f2ed6))
    - Merge branch 'main' into pathspec ([`7b61506`](https://github.com/Byron/gitoxide/commit/7b615060712565f515515e35a3e8346278ad770c))
    - make fmt ([`47724c0`](https://github.com/Byron/gitoxide/commit/47724c0edb382c036a3fc99884becfd2b0740d4b))
</details>

## 0.0.2 (2022-07-22)

### New Features

 - <csr-id-c76fde7de278b49ded13b655d5345e4eb8c1b134/> initialize `Time` from `now_utc` and `now_local`
   Localtime support depends on some other factors now, but that
   will only get better over time.
   
   We might have to document `unsound_local_time` at some point.
 - <csr-id-aeda76ed500d2edba62747d667227f2664edd267/> `Time::is_set()` to see if the time is more than just the default.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 8 commits contributed to the release over the course of 32 calendar days.
 - 39 days passed between releases.
 - 2 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 1 unique issue was worked on: [#331](https://github.com/Byron/gitoxide/issues/331)

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **[#331](https://github.com/Byron/gitoxide/issues/331)**
    - initialize `Time` from `now_utc` and `now_local` ([`c76fde7`](https://github.com/Byron/gitoxide/commit/c76fde7de278b49ded13b655d5345e4eb8c1b134))
    - `Time::is_set()` to see if the time is more than just the default. ([`aeda76e`](https://github.com/Byron/gitoxide/commit/aeda76ed500d2edba62747d667227f2664edd267))
 * **Uncategorized**
    - Release gix-hash v0.9.6, gix-features v0.22.0, gix-date v0.0.2, gix-actor v0.11.0, gix-glob v0.3.1, gix-path v0.4.0, gix-attributes v0.3.0, gix-tempfile v2.0.2, gix-object v0.20.0, gix-ref v0.15.0, gix-sec v0.3.0, gix-config v0.6.0, gix-credentials v0.3.0, gix-diff v0.17.0, gix-discover v0.3.0, gix-index v0.4.0, gix-mailmap v0.3.0, gix-traverse v0.16.0, gix-pack v0.21.0, gix-odb v0.31.0, gix-url v0.7.0, gix-transport v0.19.0, gix-protocol v0.18.0, gix-revision v0.3.0, gix-worktree v0.4.0, git-repository v0.20.0, gix-commitgraph v0.8.0, gitoxide-core v0.15.0, gitoxide v0.13.0, safety bump 22 crates ([`4737b1e`](https://github.com/Byron/gitoxide/commit/4737b1eea1d4c9a8d5a69fb63ecac5aa5d378ae5))
    - prepare changelog prior to release ([`3c50625`](https://github.com/Byron/gitoxide/commit/3c50625fa51350ec885b0f38ec9e92f9444df0f9))
    - Merge branch 'config-cascade' ([`f144eaf`](https://github.com/Byron/gitoxide/commit/f144eaf5863ae5cac63103f0db51c35fcf03a948))
    - Merge pull request #1 from Byron/main ([`085e76b`](https://github.com/Byron/gitoxide/commit/085e76b121291ed9bd324139105d2bd4117bedf8))
    - Merge branch 'main' into pathspec ([`89ea12b`](https://github.com/Byron/gitoxide/commit/89ea12b558bcc056b892193ee8fb44b8664b5da4))
    - Merge branch 'main' into cont_include_if ([`41ea8ba`](https://github.com/Byron/gitoxide/commit/41ea8ba78e74f5c988148367386a1f4f304cb951))
</details>

## 0.0.1 (2022-06-13)

### New Features

 - <csr-id-cfb6a726ddb763f7c22688f8ef309e719c2dfce4/> Add `Time` type.
   It was originally from the `gix-actor` crate.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 6 commits contributed to the release over the course of 57 calendar days.
 - 59 days passed between releases.
 - 1 commit was understood as [conventional](https://www.conventionalcommits.org).
 - 1 unique issue was worked on: [#427](https://github.com/Byron/gitoxide/issues/427)

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **[#427](https://github.com/Byron/gitoxide/issues/427)**
    - reflog lookup by date is complete ([`b3d009e`](https://github.com/Byron/gitoxide/commit/b3d009e80e3e81afd3d095fa2d7b5fc737d585c7))
    - Add `Time` type. ([`cfb6a72`](https://github.com/Byron/gitoxide/commit/cfb6a726ddb763f7c22688f8ef309e719c2dfce4))
 * **Uncategorized**
    - Release gix-date v0.0.1, gix-hash v0.9.5, gix-features v0.21.1, gix-actor v0.10.1, gix-path v0.2.0, gix-attributes v0.2.0, gix-ref v0.14.0, gix-sec v0.2.0, gix-config v0.5.0, gix-credentials v0.2.0, gix-discover v0.2.0, gix-pack v0.20.0, gix-odb v0.30.0, gix-url v0.6.0, gix-transport v0.18.0, gix-protocol v0.17.0, gix-revision v0.2.1, gix-worktree v0.3.0, git-repository v0.19.0, safety bump 13 crates ([`a417177`](https://github.com/Byron/gitoxide/commit/a41717712578f590f04a33d27adaa63171f25267))
    - update changelogs prior to release ([`bb424f5`](https://github.com/Byron/gitoxide/commit/bb424f51068b8a8e762696890a55ab48900ab980))
    - Merge branch 'revspec-parsing' ([`a2c8969`](https://github.com/Byron/gitoxide/commit/a2c8969ba821fd387c39b14248074767f54749c8))
    - Merge branch 'main' into repo-status ([`0eb2372`](https://github.com/Byron/gitoxide/commit/0eb23721dca78f6e6bf864c5c3a3e44df8b419f0))
</details>

## 0.0.0 (2022-04-14)

An empty crate without any content to reserve the name for the gitoxide project.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 2 commits contributed to the release.
 - 0 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 1 unique issue was worked on: [#331](https://github.com/Byron/gitoxide/issues/331)

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **[#331](https://github.com/Byron/gitoxide/issues/331)**
    - frame for gix-date ([`37e8ef8`](https://github.com/Byron/gitoxide/commit/37e8ef890305db0798059919290a0d27a9a39194))
 * **Uncategorized**
    - Release gix-date v0.0.0 ([`2bc2f76`](https://github.com/Byron/gitoxide/commit/2bc2f765dc4f8a4779c132f7729fb782c66c0d99))
</details>
