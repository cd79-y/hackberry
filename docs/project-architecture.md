# 義手システム構成

## Step 1: HACKberry基本動作

```text
[手動入力]
    ↓
[制御基板 / MCU]
    ↓
[モータ / アクチュエータ]
    ↓
[HACKberry Hand]
```

## 拡張後

```text
[EMG Sensor] ─────→ [MCU] ─────→ [Actuator] ─────→ [HACKberry Hand]
                      ↑                               │
                      │                               ↓
                [PC / Unity] ←────── [Contact / Pressure Sensor]
                      │
                      └────────────→ [Haptic Feedback]
```

## モジュール分離
- **Mechanics**: HACKberry機構・3Dプリント部品
- **Actuation**: モータ、ワイヤ、駆動系
- **Control**: MCU、制御ロジック
- **Sensing**: EMG、接触、圧力
- **Feedback**: 振動などの触覚提示
- **XR Interface**: PC / Unityとの通信
