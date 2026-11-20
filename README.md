## Nikolai Tsyrenov

Solo developer. On-device ML, mobile apps, and networking tools. Most of what I open-source is
the part that was hard to get right: protocols, conversion recipes, datasets.

### Networking and censorship circumvention

- **[farvater-core](https://github.com/tsyrenov1987/farvater-core)**: the routing core of the
  Farvater VPN client, in Go. It picks a path by proven delivery instead of ping, because a
  throttled path answers a probe fast and then delivers nothing. It also contains **Kilvater**,
  a tunnel protocol that looks like an ordinary HTTPS site: spec in
  [docs/KILVATER.md](https://github.com/tsyrenov1987/farvater-core/blob/main/docs/KILVATER.md),
  server `kilvaterd`, test vectors and an independent Python reference implementation. Apache-2.0.
- **[provenpath](https://github.com/tsyrenov1987/provenpath)**: the same delivery-first path
  ordering as a dependency-free Kotlin library for sing-box and clash style clients. Apache-2.0.

### Messenger

- **Nyutag**, a Matrix messenger with its own client engine and no third-party libraries:
  [iOS](https://github.com/tsyrenov1987/nyutag-ios) (Swift),
  [Android](https://github.com/tsyrenov1987/nyutag-android) (Kotlin).

### On-device ML

- **[demucs-coreml-ios](https://github.com/tsyrenov1987/demucs-coreml-ios)**: Demucs v4 on
  iPhone. Core ML conversion plus the STFT/iSTFT half Core ML cannot do, golden-tested against
  PyTorch.
- **[coreml-photo-restoration](https://github.com/tsyrenov1987/coreml-photo-restoration)**:
  PyTorch to Core ML recipes for colorization, face restoration, inpainting and upscaling, with
  the quantization settings that survive the Neural Engine and the ones that do not.
- **[unity-llamacpp-ios](https://github.com/tsyrenov1987/unity-llamacpp-ios)**: llama.cpp inside
  a Unity game on iOS. Static Metal build, a C ABI IL2CPP can call, GBNF-constrained output.
- **[RussianG2P](https://github.com/tsyrenov1987/RussianG2P)**: Russian text to IPA phonemes in
  Swift. Rule-based, deterministic, zero dependencies.

### Open datasets (CC BY 4.0)

- **[car-maintenance-schedules](https://github.com/tsyrenov1987/car-maintenance-schedules)**:
  service schedules by make and model (oil, tires, brakes, timing belt vs chain, milestones).
- **[manufacturer-warranty-terms](https://github.com/tsyrenov1987/manufacturer-warranty-terms)**:
  standard manufacturer warranty terms by brand (length, how to claim, registration).
- **[zurkhai-lunar-calendar](https://github.com/tsyrenov1987/zurkhai-lunar-calendar)**:
  Tibetan-Mongolian lunar calendar 2026–2027, one row per day (lunar day, element, animal, haircut days in EN/RU/MN).
