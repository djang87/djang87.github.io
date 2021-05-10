---
layout: defaults/page
permalink: index.html
narrow: false
title: PwnLab (폰랩) 소개
---

저희 연구실에서는 악성코드, 해킹, 및 그와 관련된 다양한 공격/방어 기술들을 연구합니다. 다음은 저희 연구실에서 관심을 가지는 키워드들입니다.

***#Fuzzing, #Binary Analysis, #Memory Exploitation, #Compiler/LLVM, #OS/Rootkit, #Network Security, #Block Chain, #Web Hacking, #Virtualization/Emulation, #CTF, #Wargame, #Bug Hunting, #Malware Forensic***

<br>

**퍼징 (Fuzzing)** 은 소프트웨어의 메모리 보안취약점을 자동탐색하는 기술로서 저희 연구실에서 가장 관심을 가지고 연구하는 분야중 하나입니다. 아래는 AFL 퍼저가 작동하는 모습입니다.<br>
![](./afl_screen.png){:width="100%"}
<br><br>
메모리 보안취약점은 악성코드가 몰래 침투할 수 있는 통로가 됩니다. 악성코드는 초기단계에서 소프트웨어의 사용자가 모르게 매우작은 데이터 조각인 **'쉘코드' (Shellcode)** 의 형태로 컴퓨터에 침투합니다. 아래는 Windows 쉘코드의 예시입니다.<br>
![](./shellcode.png){:width="100%"}
<br><br>
이러한 쉘코드는 최종적으로 랜섬웨어와 같은 완전한 악성코드로 바뀝니다. 악성코드는 다양한 종류가 있는데, 랜섬웨어의 경우 사용자의 중요 파일들을 암호화하여 인질로 잡아 복원의 댓가로 돈을 요구하게 됩니다. 이러한 악성코드들은 소스코드 없이 바이너리의 형태로만 존재하기 때문에, 분석을 위해서는 바이너리 분석기술이 필요합니다. 아래는 바이너리 분석을 수행하는 도구의 예시 화면입니다.<br>
![](./ida.png){:width="100%"}
<br><br>
저희 연구실에서는 위와 같은 기본적인 컴퓨터보안이슈들에 집중하면서 LLVM, Web Assembly, Block Chain 등과 같은 새로운 기술들을 융합하는 방향으로도 연구를 수행합니다.

 <br>

## 연구원 모집

PwnLab (폰랩) 에서는 학부연구원 (단기인턴), 석/박사 대학원생 을 상시 모집하고 있습니다.
학부생연구원은 주로 특정한 프로젝트에 대해서 집중적이고 단기적인 참여를 하게됩니다.
석/박사 대학원생은 특정한 프로젝트 하나에 국한되지 않고, 학위 기간동안 다양한 방면으로 지도를 받으며 여러가지 활동을 같이 하게됩니다. 기본적으로는 논문 출판을 목표로 연구를 수행하게되며 연구 활동을 위해서 최소한의 C/Python 코딩 및 Linux 활용능력이 요구됩니다 (CTF/Wargame 에 관심이 있다면 더 좋습니다). 연구원 지원/상담 관련 문의는 djang@sungshin.ac.kr 로 이메일 주시기 바랍니다.


