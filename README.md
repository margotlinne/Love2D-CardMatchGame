# Flip The Burger

![gif](https://github.com/user-attachments/assets/acb1d2d0-675e-47d8-9328-c41a4603aa85)

![screenshot](https://github.com/user-attachments/assets/c46aa5e6-00f6-4f7f-9dbf-6f3bc8cf8327)

## About

**Flip The Burger**는 캐쥬얼 메모리 매치 업 카드 게임입니다. 3초 동안 카드의 앞면을 보여준 뒤 뒤집어서 이미지가 같은 카드 쌍을 맞춰 나가는 게임입니다. R을 눌러 재시작하고, 카드를 맞출 때마다 50점을 얻고 틀릴 때마다 10점을 잃습니다. PC용으로 빌드되었습니다.

**Flip The Burger** is a casual memory-matching game where players flip two cards at a time to find matching pairs. Pressing "R" allows the game to restart. Players earn 50 points for a correct match and lose 10 points for an incorrect guess. The game is built for PC.

<br>

## Information

- **Framework**: Love2D(Lua)
- **Platform**: PC
- **Team Size**: 1
- **Time Frame**: 1 week
  
<br> 

## Features
시스템	| 설명
:--- | :---
🃏 카드 매칭 <br><br> Card Matching	| 16쌍의 햄버거 재료 카드 매칭. 정답 시 제거, 오답 시 다시 가림 <br><br> Match 16 pairs of burger ingredients. Correct pairs disappear; incorrect ones are flipped back.
🖱️ 마우스 인터랙션 <br><br> Mouse Interaction |	마우스로 카드 선택 및 뒤집기 <br><br> Select and flip cards with mouse clicks
🔊 사운드 효과 <br><br> Sound Effects	| 카드 뒤집기 시 앞면/뒷면 효과음 재생 <br><br> Sound effects on flipping cards
🎯 점수 시스템 <br><br> Score System | 정답 시 +50점, 오답 시 -10점 <br><br> +50 points for correct match, -10 for wrong
🕓 제한 시간 공개 <br><br> Limited Preview	 | 시작 시 모든 카드를 잠시 보여준 후 자동으로 숨김 <br><br> All cards are revealed briefly at start, then hidden

<br>

## Key Points

- **카드 위치 무작위 배치**: setRandomValue() 및 setIndex()를 통해 매 판마다 카드 위치가 다름 <br> **Randomized Card Placement**: Cards are shuffled every round using custom logic

- **단순한 구조지만 완결된 흐름**: 시작 → 카드 선택 → 정답/오답 판정 → 점수 → 종료까지 자연스럽게 구성 <br> **Complete Game Loop**: From start to end with scoring and win condition

- **경량 구현**: Love2D 기반으로 가볍고 빠르게 실행 가능 <br> **Lightweight Build**: Runs smoothly on most machines

<br>

## Structure

```
📂 project root
├── main.lua             # Love2D 진입점 및 씬 전환 처리
│                         Entry point, handles scene switching
├── conf.lua             # 윈도우 설정
│                         Window configuration
│
├── scene/
│   ├── splash.lua       # 시작 화면 및 타이틀 효과 처리
│                         Splash screen logic
│   └── game.lua         # 카드 매칭 게임 전체 로직
│                         Full game logic (match, score, flip)
```
<br> 

#### <a href="https://www.youtube.com/watch?v=c9hruFg9UOA&list=PLVgVcpUV3wTMd91EiLjE9PvgdMCfvKSws&index=12">▶️Play Video</a>
