# Temporary encrypted Cadentide iOS build

This repository contains only an AES-256 encrypted build payload. Private
source and signing data are never committed in readable form, and no Expo or
Apple-account login session is uploaded.

The workflow decrypts the payload in an ephemeral GitHub-hosted macOS runner,
runs the native tests, builds the registered-device IPA, verifies its signature,
and publishes the resulting installation URL.
