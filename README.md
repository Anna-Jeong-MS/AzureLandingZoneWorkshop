# Azure Landing Zone Workshop

![Untitled](images/Untitled.png)

Azure 기반의 보안 중심 Landing Zone 구축 실습을 위한 워크숍 리포지토리입니다.  
이 워크숍은 Virtual WAN 기반 네트워크, Azure Firewall, WAF, 보안 경로 제어, 라우팅 구성 등을 포함하여 기업 환경에 적합한 초기 Azure 인프라를 구성하는 데 중점을 둡니다.

---

## 🎯 목표

- 보안과 거버넌스를 고려한 Azure 인프라의 기본 구조 이해  
- Virtual WAN 기반 네트워크 아키텍처 실습  
- Azure Firewall, Application Gateway, WAF를 포함한 경로 제어 흐름 구성  
- 실제 VM/Web App 등을 통해 트래픽이 흐르는 경로 검증  

---

## 🛠 워크플로우 (실습 단계)

| 단계 | 설명 |
|------|------|
| 1 | network 폴더에서 허브와 스포크 VNet, Virtual WAN 허브 배포 |
| 2 | security 폴더에서 Azure Firewall, WAF, NSG 배포 및 기본 설정 |
| 3 | connectivity 폴더에서 허브-스포크 연결, 라우팅 경로 구성 |
| 4 | workloads 폴더에서 VM/Web App 배포 |
| 5 | 트래픽 흐름 테스트 및 검증 (방화벽 통과, AppGW – Backend 통신 등) |

---

## 🔄 최신 변경 및 반영 포인트 (워크숍 기준)

- Virtual WAN 허브 라우팅 테이블을 활용한 경로 제어 (UDR 대신 Hub 라우팅 중심)  

---

## 📜 라이선스

이 워크숍 리포지토리는 **MIT 라이선스** 하에 배포됩니다. 자유롭게 수정, 배포 가능하며, 출처 표기를 부탁드립니다.  
