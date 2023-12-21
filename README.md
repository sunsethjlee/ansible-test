
# 개요
![Alt text](image.png)

## 구조 & 작동 현황
```python
.
├── blk #정상작동
│   └── tasks
│       └── main.yaml
├── change_local.yaml
├── docker 
│   └── tasks
│       └── main.yaml
├── hostname #정상작동
│   └── tasks
│       └── main.yaml
├── image.png
├── lvm #정상작동
│   ├── tasks
│   │   └── main.yaml
│   └── vars
│       └── main.yaml
├── nas
│   ├── tasks
│   │   └── main.yaml
│   └── vars
│       └── main.yaml
├── playbook.yaml
└── README.md
```

- 대상 hosts: 
    - lhj-lvm-test000 (ansibe svr) 
    - lhj-lvm-test002 (node1)
    - lhj-lvm-test003 (node2)

## 폴더 설명
task 별 폴더 생성
 - blk : 블록스토리지 생성
 - lvm : lv 생성
 - nas : nas 생성
 - hostname : hostname 변경
 - docker(미완) : 도커 설치 

- inspect(진행중): 취약점 점검 

    - [Testing Strategies](https://docs.ansible.com/ansible/latest/reference_appendices/test_strategies.html)


## docs
- [모듈 docs](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/index.html)

## 기타 참고 링크
- [개발자가 ansible 시작하기](https://wikidocs.net/130112)


## 주의사항
- 제어 노드는 Linux 나 Unix만 지원  (리눅스 기반 / window, macOS는 ansible 사용불가)
- ssh 기반으로 동작하기 때문에 에이전트를 설치할 필요 없이 ssh 접속 정보만을 주면 된다 (/etc/ansible/hosts 에 작성)
![Alt text](image-1.png)