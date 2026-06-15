# Changelog

This page tracks OpenTalking releases, capability progress, roadmap items, and compatibility notes.

## v0.1.0 - 2026-06-16

- **First GitHub Release**
  Published the initial release package for the OpenTalking orchestration layer, including API, worker, web console, and documentation-backed install paths.

- **Docker delivery**
  Added versioned GHCR image targets for `opentalking-api`, `opentalking-worker`, and `opentalking-web`.

- **Python artifacts**
  The release workflow builds and checks wheel and source distribution artifacts for GitHub Release attachment.

- **Packaging boundary**
  Model weights are not bundled in Python packages or Docker images; users should follow model-specific download and OmniRT/runtime setup docs.


## May 2026

### 2026/05/17

- **QuickTalk integration**
  QuickTalk / Wav2Lip now have easier startup paths and can be launched directly through OpenTalking for digital-human generation.

### 2026/05/15

- **MuseTalk WebRTC playback optimization**
  Added MuseTalk media backpressure to improve WebRTC playback stability.

### 2026/05/14

- **MuseTalk adaptation**
  Added the MuseTalk talking-head path for lightweight full-frame digital-human validation.

### 2026/05/13

- **Model backend decoupling**
  Decoupled `mock`, `local`, `direct_ws`, and `omnirt` at the architecture level so different models can choose different deployment backends.

### 2026/05/08

- **QuickTalk local adapter**
  Added the QuickTalk model adapter, configuration notes, and async initialization.

* * *

## April 2026

### 2026/04/16

- **Baseline real-time digital-human experience**
  Built the main Web console, LLM conversation, TTS, subtitle events, and WebRTC audio/video playback pipeline.

* * *

## Compatibility Notes

- Starting with `v0.1.0`, this changelog includes formal release sections.
- Model integration, runtime backends, and configuration keys are still evolving quickly. Check “Model Support” and “Usage Guide” before upgrading.
- Benchmark data must include hardware, model, backend, startup state, and input assets; numbers should not be compared across environments without context.
