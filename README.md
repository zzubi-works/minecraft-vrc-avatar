# Minecraft VRC Avatar

VRChat 아바타를 마인크래프트 서버용 MMD(PMX) 묶음으로 보내는 Unity 도구의 ALCOM / VCC 저장소입니다.

## 넣는 법

1. ALCOM(또는 VCC) → 설정 → 패키지 → **저장소 추가**에 아래 주소를 넣습니다.
   `https://raw.githubusercontent.com/zzubi-works/minecraft-vrc-avatar/main/index.json`
2. 아바타 프로젝트 → **패키지 관리** → `Minecraft VRC Avatar`를 설치합니다.
3. Unity 메뉴 **Tools → Minecraft VRC Avatar → 마크로 보내기** → **[마크로 보내기]**. 처음 한 번만 마크 폴더를 고릅니다.

## 들어 있는 것

| 파일 | 내용 |
|---|---|
| `index.json` | 저장소 목록. 패키지 zip 주소와 SHA-256을 담습니다 |
| Releases `v<판>` | 패키지 zip `com.zzubi-works.minecraft-vrc-avatar-<판>.zip` |

패키지는 VRChat SDK(`com.vrchat.avatars` 3.5 이상)가 든 Unity 2022.3 프로젝트에서 씁니다. 마크 쪽은 MmdSkin과 묶음을 받는 서버 모드가 있어야 합니다.
원래 셰이더로 그린 색을 텍스처에 구워 옮기고(움직이는 효과·기믹은 빠짐), 뼈·표정 몇 개·물리 근사를 옮깁니다. 물리는 쉬는 모양을 지키도록 좁게 흔들립니다.
내보낸 아바타의 권리는 원래 아바타의 약관을 따릅니다.

## 라이선스

MIT (`LICENSE`).

---

Minecraft VRC Avatar: VPM repository for a Unity editor tool that converts a VRChat avatar into an MMD (PMX) bundle for a Minecraft server.
Add `https://raw.githubusercontent.com/zzubi-works/minecraft-vrc-avatar/main/index.json` in ALCOM / VCC.

## 바뀐 것

- 0.1.1: 원래 셰이더로 색 굽기(피부·눈·털 색이 Unity와 맞음), 텍스처 없는 재질 막기, 흔들림이 멈추지 않던 물리 고침(좁은 제한·안정 스프링·큰 감쇠, 겹친 PhysBone 장치는 흔들지 않음).
- 0.1.0: 첫 판.
