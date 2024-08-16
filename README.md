서버 구성
- master 서버 3대
- worker 서버 2대
- lb 서버 1대

설치 순서

[모든 서버] 
1. /etc/yum.repos.d/CentOS-Base.repo 설정 적용.
  - 기존 /etc/yum.repos.d/CentOS-Base.repo 와 차이 확인해보기
    
2. Kubernetes Install 적용

[lb 서버]

3. multi-master 단일 진입점인 LoadBalancer 구성 (LB)
   - server ip 설정 주의 

[master 서버]

4. kubeadm 이용 HA 클러스터 구성
etcd 가 동기화 되게 하기 위한 작업
