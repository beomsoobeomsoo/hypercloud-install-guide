# HyperCloud 설치 시 주의할 점

## Ceph 설치 시 주의 사항
* ceph 설치에 device를 사용할 경우의 주의 사항입니다.
* lvm으로 묶이거나 다른 용도로 사용 중인 device는 지원되지 않으며
* ceph osd가 deploy되는 노드에 사용할 device가 반드시 존재 및 umount 상태여야 합니다.
* 따라서 클러스터 구성 전 device의 상태를 확인하고, 
* 자세한 내용은 rook-ceph 설치 단계를 참고하시기 바랍니다.

## Nvidia GPU Driver 설치 시 주의 사항
* Pod의 GPU 사용 기능을 위해 Nvidia GPU Driver 설치 시 주의 사항입니다.
* UEFI 모드로 OS를 설치 할 경우, Secure Boot(보안 부팅) 기능을 Off 하여 OS를 부팅해야합니다.