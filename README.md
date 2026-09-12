## Nikolai Tsyrenov

Solo developer. On-device ML, mobile apps, and networking tools. Most of what I open-source is
the part that was hard to get right — conversion recipes, protocol plumbing, datasets — rather
than whole products.

### Networking and censorship circumvention

- **[orden-android-client](https://github.com/tsyrenov1987/orden-android-client)** — Android VPN
  client on the sing-box core: VLESS-Reality and Hysteria2/Salamander with automatic per-node
  failover, on-device, no logs. Takes any subscription URL or share link. MIT.
  Runs the client side of [joinorden.com](https://joinorden.com).
- **[orden-singbox-configs](https://github.com/tsyrenov1987/orden-singbox-configs)** — Production
  sing-box config: VLESS-Reality ↔ Hysteria2 auto-failover plus a Russian split-tunnel that keeps
  banks and government services on a real local IP. Six production gotchas explained.
- **[provenpath](https://github.com/tsyrenov1987/provenpath)** — Kotlin library that orders proxy
  paths by proven delivery instead of latency, because `urltest` measures a `HEAD` request and a
  throttled path answers fast while delivering nothing. Apache-2.0.

### On-device ML

- **[demucs-coreml-ios](https://github.com/tsyrenov1987/demucs-coreml-ios)** — Run Demucs v4 on
  iPhone: Core ML conversion plus the STFT/iSTFT half Core ML cannot do, golden-tested against
  PyTorch.
- **[coreml-photo-restoration](https://github.com/tsyrenov1987/coreml-photo-restoration)** —
  PyTorch to Core ML recipes for colorization, face restoration, inpainting and upscaling,
  including the quantization settings that survive the Neural Engine and the ones that do not.
- **[unity-llamacpp-ios](https://github.com/tsyrenov1987/unity-llamacpp-ios)** — llama.cpp inside
  a Unity game on iOS: static Metal build, a C ABI IL2CPP can call, GBNF-constrained output.
- **[RussianG2P](https://github.com/tsyrenov1987/RussianG2P)** — Russian text to IPA phonemes in
  Swift. Rule-based, deterministic, zero dependencies — the G2P step that until now only existed
  in Python.

### Open datasets (CC BY 4.0)

- **[car-maintenance-schedules](https://github.com/tsyrenov1987/car-maintenance-schedules)** —
  Service schedules by make and model: oil, tires, brakes, timing belt vs chain, milestones.
- **[manufacturer-warranty-terms](https://github.com/tsyrenov1987/manufacturer-warranty-terms)** —
  Standard manufacturer warranty terms by brand: length, how to claim, registration.
