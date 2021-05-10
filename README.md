> # **Leader's Head**

### **Initialized By SeongKyeong Yoon**

<hr>

<br>

> ## **Background**

<br>

### **매일매일 수많은 정보가 생겨나지만, 우리는 모든 정보를 확인할 여유가 없습니다**

#### **세상의 모든 정보를 일일이 찾아보는게 어려운 지금, 관심 있는 정보의 헤드라인이 한눈에 보인다면 멋지지 않을까요?**

#### **여러 소식들을 한눈에 확인할 수 있도록 Compact & Powerful Dashboard를 만들어서 서비스하려고 합니다.**

<hr>

<br>

> ## **Mission**

<br>

### **가능한 모든 Information Source를 통합해서 매일 최신 정보를 Scrape & Update한다**

- **주요 나라의 뉴스, 부동산, 유튜브, 주요 정보 등의 headline과 함께 카테고리, content link를 받아오고 정리한다.**
- **통합된 UI로 한눈에 뉴스들을 볼 수 있도록 정리해준다.**
- **적절한 Processing을 통해서 주요 뉴스, 연관 뉴스, 키워드 추출, 검색 등의 서비스를 제공한다.**
- **누구나 쉽게 새로운 소스를 통합할 수 있도록 General Interface를 제공한다.**

<hr>

<br>

> ## **Requirement**

<br>

##### **`Server`**

- **다양한 information source를 unified interface로 통합할 수 있다.**
- **동시에 다양한 data source에서 정보를 받아올 수 있다.**
- **안정적이고 효과적으로 ELT를 진행한다.**
- **코드 변경, 모듈 추가가 자유롭고 관리가 쉽도록 시스템을 설계한다.**
- **Component 설계 이후 어떤 언어와 프레임워크로 구현할 지 결정한다**
- **다양한 workload를 control하는 Coordinator와 실제 task를 handling하는 Worker로 구성된다.**
- **언어 및 프레임워크 등에 제한되지 않도록 decoupled system을 구성한다.**
- **TDD를 통해 안정적인 CI 환경을 제공한다.**
- **시스템을 잘 설명한 Documentation을 관리한다.**

##### **`Datalake`**

- **비용 효율적인 Data Loading을 위해 Object Storage의 한 종류인 AWS S3를 사용한다.**

##### **`Database`**

- **Writing이 적고, Reading이 main이 되는 Usecase, 시간이 지나면 접근이 줄어들고 특정 패턴의 정보가 자주 검색되는 Usecase에 맞는 DB 및 Data System를 찾고 설계한다.**

##### **`Client`**

- **많은 양의 데이터를 쉽고 직관적으로 확인할 수 있도록 UI를 설계한다.**
- **많은 양의 데이터를 효율적으로 다룰 수 있는 구조로 클라이언트를 설계 및 최적화한다.**
- **유저 입장에서 빠르고 간편하게 원하는 주제의 도움되는 정보를 쉽게 찾을 수 있도록 reactive 검색 기능을 개발한다.**
- **코드 변경, 모듈 추가가 자유롭고 관리가 쉽도록 시스템을 설계한다.**
- **Authentication / Authorization / Security 를 제공한다**
- **시스템을 잘 설명한 Documentation을 관리한다.**

##### **`Infra`**

- **개발과 배포를 연결한 CI/CD를 구현해서 일관되고 안정된 환경을 보장한다.**
- **Infra As A Code를 구현한 AWS CDK를 이용해서 모든 스택을 AWS 위에 배포한다.**
- **항상 어떤 환경에서든 배포할 수 있도록 Documentation & Instruction을 작성한다.**

<hr>

<br>

> ## **Progress**

<br>

##### **`2021-05-11`**

- **Project Initializatoin**
- **Use Case Design**
- **High Level Design 및 Component Design**
- **어떤 Tool과 모듈을 사용하면 좋을지 탐색**
