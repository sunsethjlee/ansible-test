![Alt text](img/image.png)

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
 # 설치 환경
OS : Ubuntu 16.04

대상 hosts: 
- lhj-lvm-test000 (ansibe svr) 
- lhj-lvm-test002 (node1) 10.0.200.7
- lhj-lvm-test003 (node2) 10.0.200.8


## 폴더 설명
task 별 폴더 생성
 - blk : 블록스토리지 생성
 - lvm : lv 생성
 - nas : nas 생성
 - hostname : hostname 변경
 - docker(미완) : 도커 설치 

- inspect(진행중): 취약점 점검 

    - [Testing Strategies](https://docs.ansible.com/ansible/latest/reference_appendices/test_strategies.html)




