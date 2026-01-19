<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>모바일 앱 QA 신입 교육 과정 - CVT QA 4주 완성</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            line-height: 1.6;
            color: #37352f;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        .header {
            background: white;
            border-radius: 16px;
            padding: 60px 40px;
            text-align: center;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.1);
            margin-bottom: 40px;
        }

        .header h1 {
            font-size: 3em;
            margin-bottom: 20px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .header .subtitle {
            font-size: 1.3em;
            color: #666;
            margin-bottom: 30px;
        }

        .badges {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }

        .badge {
            display: inline-block;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9em;
            font-weight: 600;
            color: white;
        }

        .badge-blue { background: #0066cc; }
        .badge-green { background: #059669; }
        .badge-orange { background: #ea580c; }
        .badge-red { background: #dc2626; }

        .quick-nav {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .quick-nav a {
            color: #667eea;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s;
        }

        .quick-nav a:hover {
            color: #764ba2;
        }

        .content-card {
            background: white;
            border-radius: 16px;
            padding: 40px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.1);
            margin-bottom: 30px;
        }

        h2 {
            font-size: 2em;
            margin-bottom: 20px;
            color: #667eea;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        h3 {
            font-size: 1.5em;
            margin: 30px 0 15px 0;
            color: #37352f;
        }

        h4 {
            font-size: 1.2em;
            margin: 20px 0 10px 0;
            color: #555;
        }

        .intro-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .intro-card {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 25px;
            border-radius: 12px;
            border-left: 4px solid #667eea;
        }

        .intro-card h4 {
            margin-top: 0;
            color: #667eea;
        }

        .week-card {
            background: white;
            border: 2px solid #e5e7eb;
            border-radius: 12px;
            padding: 30px;
            margin-bottom: 30px;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .week-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
        }

        .week-card.week1 { border-left: 6px solid #0066cc; }
        .week-card.week2 { border-left: 6px solid #7c3aed; }
        .week-card.week3 { border-left: 6px solid #059669; }
        .week-card.week4 { border-left: 6px solid #dc2626; }

        .week-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        .week-title {
            font-size: 1.8em;
            margin: 0;
        }

        .week1 .week-title { color: #0066cc; }
        .week2 .week-title { color: #7c3aed; }
        .week3 .week-title { color: #059669; }
        .week4 .week-title { color: #dc2626; }

        .week-links {
            display: flex;
            gap: 10px;
        }

        .week-link {
            padding: 8px 16px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
            font-size: 0.9em;
        }

        .md-link {
            background: #f3f4f6;
            color: #374151;
        }

        .html-link {
            background: #667eea;
            color: white;
        }

        .week-link:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }

        .week-goal {
            background: #f9fafb;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 15px;
            font-style: italic;
            color: #555;
        }

        details {
            margin: 20px 0;
            padding: 20px;
            background: #f9fafb;
            border-radius: 8px;
        }

        summary {
            cursor: pointer;
            font-weight: 700;
            font-size: 1.1em;
            padding: 10px;
            background: white;
            border-radius: 8px;
            user-select: none;
        }

        summary:hover {
            background: #f3f4f6;
        }

        .day-list {
            margin-top: 15px;
            padding-left: 20px;
        }

        .day-item {
            margin: 10px 0;
            padding-left: 10px;
            border-left: 3px solid #d1d5db;
        }

        .deliverable-list {
            list-style: none;
            padding-left: 0;
        }

        .deliverable-list li {
            padding: 8px 0 8px 30px;
            position: relative;
        }

        .deliverable-list li:before {
            content: "☐";
            position: absolute;
            left: 0;
            font-size: 1.2em;
            color: #667eea;
        }

        .table-container {
            overflow-x: auto;
            margin: 20px 0;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            background: white;
            border-radius: 8px;
            overflow: hidden;
        }

        th {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 15px;
            text-align: left;
            font-weight: 600;
        }

        td {
            padding: 15px;
            border-bottom: 1px solid #e5e7eb;
        }

        tr:hover {
            background: #f9fafb;
        }

        .roadmap {
            background: #1e293b;
            color: white;
            padding: 30px;
            border-radius: 12px;
            margin: 20px 0;
            font-family: 'Courier New', monospace;
            overflow-x: auto;
        }

        .roadmap pre {
            margin: 0;
            color: #10b981;
            line-height: 1.8;
        }

        .checklist-section {
            margin: 20px 0;
        }

        .checklist-category {
            background: white;
            border-radius: 8px;
            padding: 20px;
            margin-bottom: 20px;
            border-left: 4px solid #667eea;
        }

        .checklist-category h3 {
            margin-top: 0;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .checklist-category ul {
            list-style: none;
            padding-left: 0;
        }

        .checklist-category li {
            padding: 8px 0 8px 30px;
            position: relative;
        }

        .checklist-category li:before {
            content: "☐";
            position: absolute;
            left: 0;
            font-size: 1.2em;
            color: #667eea;
        }

        .tip-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }

        .tip-card {
            background: white;
            border-radius: 12px;
            padding: 25px;
            border-top: 4px solid #667eea;
        }

        .tip-card h3 {
            margin-top: 0;
            color: #667eea;
        }

        .tip-card ul {
            padding-left: 20px;
        }

        .tip-card li {
            margin: 8px 0;
        }

        .contact-section {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px;
            border-radius: 12px;
            margin: 20px 0;
        }

        .contact-section h3 {
            color: white;
            margin-top: 0;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .contact-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 8px;
        }

        .footer {
            background: white;
            border-radius: 16px;
            padding: 40px;
            text-align: center;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.1);
            margin-top: 40px;
        }

        .footer h3 {
            color: #667eea;
            margin-bottom: 20px;
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 20px;
            flex-wrap: wrap;
        }

        .footer-links a {
            color: #667eea;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s;
        }

        .footer-links a:hover {
            color: #764ba2;
        }

        @media (max-width: 768px) {
            .header h1 {
                font-size: 2em;
            }

            .header .subtitle {
                font-size: 1.1em;
            }

            .content-card {
                padding: 20px;
            }

            .intro-grid {
                grid-template-columns: 1fr;
            }

            .week-header {
                flex-direction: column;
                align-items: flex-start;
                gap: 15px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header Section -->
        <div class="header">
            <h1>📚 모바일 앱 QA 신입 교육 과정</h1>
            <p class="subtitle">CVT QA 엔지니어를 위한 4주 완성 커리큘럼</p>
            
            <div class="badges">
                <span class="badge badge-blue">Duration: 4 Weeks</span>
                <span class="badge badge-green">Level: Beginner</span>
                <span class="badge badge-orange">Format: Hands-on</span>
                <span class="badge badge-red">Language: Korean</span>
            </div>

            <div class="quick-nav">
                <a href="#week1">Week 1</a> •
                <a href="#week2">Week 2</a> •
                <a href="#week3">Week 3</a> •
                <a href="#week4">Week 4</a> •
                <a href="#resources">Resources</a>
            </div>
        </div>

        <!-- Introduction -->
        <div class="content-card">
            <h2>📋 과정 소개</h2>
            <p style="font-size: 1.1em; margin: 20px 0;">
                본 교육 과정은 <strong>모바일 앱 QA 신입 사원</strong>을 대상으로 하는 <strong>4주 집중 교육 프로그램</strong>입니다.
            </p>

            <h3>✨ 교육 목표</h3>
            <div class="intro-grid">
                <div class="intro-card">
                    <h4>📱 모바일 앱 QA 기초</h4>
                    <p>Android/iOS 앱 테스트의 핵심 개념 습득</p>
                </div>
                <div class="intro-card">
                    <h4>🔍 체계적 테스트 설계</h4>
                    <p>UI 분해부터 E2E 시나리오까지 단계별 학습</p>
                </div>
                <div class="intro-card">
                    <h4>🐛 결함 관리</h4>
                    <p>발견-보고-트리아지-수정 검증의 전체 생명주기 이해</p>
                </div>
                <div class="intro-card">
                    <h4>🚀 실전 CVT 운영</h4>
                    <p>실제 릴리스 검증 프로세스 시뮬레이션</p>
                </div>
            </div>

            <h3>📊 교육 방식</h3>
            <div class="intro-grid">
                <div class="intro-card">
                    <h4>⏱️ 학습 시간</h4>
                    <p><strong>하루 90분</strong></p>
                    <ul style="margin-top: 10px;">
                        <li>이론: 30분</li>
                        <li>실습: 60분</li>
                    </ul>
                </div>
                <div class="intro-card">
                    <h4>📅 진행 기간</h4>
                    <p><strong>총 4주 (20일)</strong></p>
                    <ul style="margin-top: 10px;">
                        <li>주당 5일 학습</li>
                        <li>주말 복습/과제</li>
                    </ul>
                </div>
                <div class="intro-card">
                    <h4>🎯 학습 방법</h4>
                    <p><strong>Hands-on 중심</strong></p>
                    <ul style="margin-top: 10px;">
                        <li>실제 앱으로 실습</li>
                        <li>매일 산출물 제출</li>
                    </ul>
                </div>
                <div class="intro-card">
                    <h4>✅ 평가 방식</h4>
                    <p><strong>산출물 기반</strong></p>
                    <ul style="margin-top: 10px;">
                        <li>일일 과제</li>
                        <li>주간 프로젝트</li>
                        <li>최종 CVT 리포트</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Week 1 -->
        <div class="content-card">
            <h2 id="week1">📅 4주 교육 커리큘럼</h2>
            
            <div class="week-card week1">
                <div class="week-header">
                    <h3 class="week-title">📘 Week 1: 기초 개념 및 도구 습득</h3>
                    <div class="week-links">
                        <a href="CVT_QA_Week1_Detailed.md" class="week-link md-link">📄 Markdown</a>
                        <a href="CVT_QA_Week1_Detailed.html" class="week-link html-link">🌐 HTML</a>
                    </div>
                </div>

                <div class="week-goal">
                    <strong>학습 목표:</strong> 모바일 앱 QA의 기본 개념을 이해하고 필수 도구를 활용할 수 있다.
                </div>

                <details>
                    <summary>📝 상세 커리큘럼 보기</summary>
                    <div class="day-list">
                        <div class="day-item">
                            <strong>Day 1: 모바일 앱 QA 입문</strong>
                            <ul>
                                <li>모바일 앱 QA의 역할과 책임</li>
                                <li>Android vs iOS 플랫폼 차이점</li>
                                <li>QA 생명주기 이해</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 2: 개발 환경 구성</strong>
                            <ul>
                                <li>Android Studio & Xcode 설치</li>
                                <li>ADB (Android Debug Bridge) 활용</li>
                                <li>iOS 시뮬레이터 & 실기기 연결</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 3: UI 부품 분류 체계</strong>
                            <ul>
                                <li>6가지 UI 컴포넌트 타입 (Button, Input, List, Dialog, Navigation, Custom)</li>
                                <li>4가지 상태 모델 (Normal, Disabled, Loading, Error)</li>
                                <li>실습: 샘플 앱 UI 분류표 작성</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 4: 테스트 케이스 작성 & 실행</strong>
                            <ul>
                                <li>테스트 케이스 구조 (Precondition, Steps, Expected Result)</li>
                                <li>테스트 실행 및 결과 기록</li>
                                <li>Pass/Fail 판정 기준</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 5: 결함 보고 기초</strong>
                            <ul>
                                <li>좋은 버그 리포트의 조건</li>
                                <li>JIRA/Bugzilla 사용법</li>
                                <li>첫 버그 리포트 작성 실습</li>
                            </ul>
                        </div>
                    </div>

                    <h4 style="margin-top: 20px;">📦 주간 산출물</h4>
                    <ul class="deliverable-list">
                        <li>환경 구성 인증서 (스크린샷)</li>
                        <li>UI 분류표 (최소 20개 컴포넌트)</li>
                        <li>테스트 실행 결과서 (5개 이상 케이스)</li>
                        <li>버그 리포트 3건 이상</li>
                        <li>Mini-Project: 간단한 앱 전체 화면 UI 분류</li>
                    </ul>
                </details>
            </div>

            <!-- Week 2 -->
            <div class="week-card week2">
                <div class="week-header">
                    <h3 class="week-title">📗 Week 2: 화면 분해 및 테스트 설계</h3>
                    <div class="week-links">
                        <a href="CVT_QA_Week2_Detailed.md" class="week-link md-link">📄 Markdown</a>
                        <a href="CVT_QA_Week2_Detailed.html" class="week-link html-link">🌐 HTML</a>
                    </div>
                </div>

                <div class="week-goal">
                    <strong>학습 목표:</strong> 복잡한 화면을 체계적으로 분석하고 효율적인 테스트를 설계할 수 있다.
                </div>

                <details>
                    <summary>📝 상세 커리큘럼 보기</summary>
                    <div class="day-list">
                        <div class="day-item">
                            <strong>Day 6: 화면 라우팅 분석</strong>
                            <ul>
                                <li>Navigation Flow 다이어그램 작성</li>
                                <li>화면 전환 시나리오 (Push, Pop, Replace, Modal)</li>
                                <li>딥링크 & 알림 처리</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 7: 데이터 흐름 추적</strong>
                            <ul>
                                <li>Local Storage vs Server Sync</li>
                                <li>데이터 동기화 오류 패턴</li>
                                <li>캐시 무효화 테스트</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 8: 조합 테스트 설계</strong>
                            <ul>
                                <li>3축 조합 (플랫폼 × 네트워크 × 로그인 상태)</li>
                                <li>2×2×2 = 8가지 시나리오 테스트</li>
                                <li>Pairwise Testing 기법</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 9: E2E 시나리오 작성</strong>
                            <ul>
                                <li>사용자 여정(User Journey) 정의</li>
                                <li>Critical Path 식별</li>
                                <li>Happy Path vs Error Path</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 10: 테스트 설계 문서화</strong>
                            <ul>
                                <li>테스트 계획서 구조</li>
                                <li>테스트 범위 정의</li>
                                <li>리스크 분석 및 우선순위</li>
                            </ul>
                        </div>
                    </div>

                    <h4 style="margin-top: 20px;">📦 주간 산출물</h4>
                    <ul class="deliverable-list">
                        <li>화면 플로우 다이어그램 (10개 이상 화면)</li>
                        <li>데이터 흐름 맵 (3개 이상 기능)</li>
                        <li>조합 테스트 표 (8가지 시나리오)</li>
                        <li>E2E 시나리오 5개 이상</li>
                        <li>Mini-Project: 실제 앱의 테스트 설계 문서</li>
                    </ul>
                </details>
            </div>

            <!-- Week 3 -->
            <div class="week-card week3">
                <div class="week-header">
                    <h3 class="week-title">📕 Week 3: 결함 발견 및 보고</h3>
                    <div class="week-links">
                        <a href="CVT_QA_Week3_Detailed.md" class="week-link md-link">📄 Markdown</a>
                        <a href="CVT_QA_Week3_Detailed.html" class="week-link html-link">🌐 HTML</a>
                    </div>
                </div>

                <div class="week-goal">
                    <strong>학습 목표:</strong> 체계적인 결함 탐색 방법을 습득하고 효과적으로 보고할 수 있다.
                </div>

                <details>
                    <summary>📝 상세 커리큘럼 보기</summary>
                    <div class="day-list">
                        <div class="day-item">
                            <strong>Day 11: 탐색적 테스팅 (Exploratory Testing)</strong>
                            <ul>
                                <li>Session-Based Test Management</li>
                                <li>Charter 작성 및 실행</li>
                                <li>Time-Boxed Testing</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 12: 재현 가능한 버그 보고</strong>
                            <ul>
                                <li>7가지 필수 항목 (Title, Steps, Expected, Actual, Environment, Severity, Attachments)</li>
                                <li>100% 재현율 달성 방법</li>
                                <li>스크린 레코딩 & 로그 첨부</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 13: Severity vs Priority</strong>
                            <ul>
                                <li>Severity 4단계 (Critical, High, Medium, Low)</li>
                                <li>Priority 3단계 (P0, P1, P2)</li>
                                <li>실전 사례 분석</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 14: 버그 트리아지 시뮬레이션</strong>
                            <ul>
                                <li>트리아지 회의 역할 (QA, Dev, PM)</li>
                                <li>버그 상태 관리 (Open, In Progress, Fixed, Closed)</li>
                                <li>Re-test & Verification</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 15: 리그레션 테스팅</strong>
                            <ul>
                                <li>리그레션 테스트 체크리스트 작성</li>
                                <li>자동화 vs 수동 테스트 판단</li>
                                <li>Side-Effect 탐지 방법</li>
                            </ul>
                        </div>
                    </div>

                    <h4 style="margin-top: 20px;">📦 주간 산출물</h4>
                    <ul class="deliverable-list">
                        <li>탐색적 테스팅 Charter 3개 이상</li>
                        <li>재현 가능한 버그 리포트 5건 이상 (100% 재현율)</li>
                        <li>트리아지 시뮬레이션 결과</li>
                        <li>리그레션 테스트 체크리스트 (20개 항목)</li>
                        <li>Mini-Project: 10개 버그 포트폴리오</li>
                    </ul>
                </details>
            </div>

            <!-- Week 4 -->
            <div class="week-card week4">
                <div class="week-header">
                    <h3 class="week-title">📙 Week 4: 실전 CVT 운영</h3>
                    <div class="week-links">
                        <a href="CVT_QA_Week4_Detailed.md" class="week-link md-link">📄 Markdown</a>
                        <a href="CVT_QA_Week4_Detailed.html" class="week-link html-link">🌐 HTML</a>
                    </div>
                </div>

                <div class="week-goal">
                    <strong>학습 목표:</strong> 실제 릴리스 검증 프로세스를 경험하고 CVT 리포트를 작성할 수 있다.
                </div>

                <details>
                    <summary>📝 상세 커리큘럼 보기</summary>
                    <div class="day-list">
                        <div class="day-item">
                            <strong>Day 16: CVT 계획 수립</strong>
                            <ul>
                                <li>CVT (Customer Validation Test) 정의</li>
                                <li>테스트 범위 결정 (7가지 핵심 질문)</li>
                                <li>리소스 & 일정 산정</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 17: Smoke Test & Sanity Test</strong>
                            <ul>
                                <li>Smoke Test 체크리스트 (핵심 기능 10개)</li>
                                <li>Build Acceptance Test</li>
                                <li>빠른 Go/No-Go 판단</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 18: E2E 테스트 실행</strong>
                            <ul>
                                <li>우선순위 기반 테스트 실행</li>
                                <li>실시간 이슈 트래킹</li>
                                <li>Blocker 이슈 에스컬레이션</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 19: 결함 처리 & 재검증</strong>
                            <ul>
                                <li>수정된 빌드 검증</li>
                                <li>Side-Effect 테스트</li>
                                <li>Regression Test 실행</li>
                            </ul>
                        </div>
                        <div class="day-item">
                            <strong>Day 20: 최종 리포트 & Go/No-Go 결정</strong>
                            <ul>
                                <li>CVT 결과 요약 (Pass/Fail/Blocked)</li>
                                <li>남은 이슈 리스크 분석</li>
                                <li>Go/No-Go 권고안 작성</li>
                            </ul>
                        </div>
                    </div>

                    <h4 style="margin-top: 20px;">📦 최종 산출물</h4>
                    <ul class="deliverable-list">
                        <li>CVT 테스트 플랜 문서</li>
                        <li>Smoke Test 체크리스트 & 결과</li>
                        <li>E2E 테스트 실행 결과 (30개 이상 케이스)</li>
                        <li>버그 트리아지 시트 (10건 이상)</li>
                        <li>재검증 로그 (Side-Effect 포함)</li>
                        <li><strong>최종 CVT 리포트</strong> (Go/No-Go 결정 포함)</li>
                    </ul>
                </details>
            </div>
        </div>

        <!-- Additional Resources -->
        <div class="content-card" id="resources">
            <h2>📚 추가 교육 자료</h2>

            <h3>📖 참고 문서</h3>
            <div class="table-container">
                <table>
                    <thead>
                        <tr>
                            <th>자료명</th>
                            <th>형식</th>
                            <th>설명</th>
                            <th>대상</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td><strong>모바일 앱 결함 분류 체계</strong></td>
                            <td>
                                <a href="MOBILE_APP_DEFECT_TAXONOMY.md" class="week-link md-link" style="margin-right: 5px;">📄 MD</a>
                                <a href="MOBILE_APP_DEFECT_TAXONOMY.html" class="week-link html-link">🌐 HTML</a>
                            </td>
                            <td>230+ 결함 유형을 7개 카테고리로 분류</td>
                            <td>중급 이상</td>
                        </tr>
                        <tr>
                            <td><strong>모바일 교육자료 #2</strong></td>
                            <td>
                                <a href="모바일%20교육자료%20#2.md" class="week-link md-link" style="margin-right: 5px;">📄 MD</a>
                                <a href="모바일_교육자료_2.html" class="week-link html-link">🌐 HTML</a>
                            </td>
                            <td>15분 Quick Start 가이드</td>
                            <td>초보자</td>
                        </tr>
                    </tbody>
                </table>
            </div>

            <p style="background: #fef3c7; padding: 15px; border-left: 4px solid #f59e0b; border-radius: 8px; margin: 20px 0;">
                💡 <strong>HTML 버전</strong>: Notion/Confluence 스타일로 제공되어 브라우저에서 바로 확인 가능합니다.
            </p>

            <h3>🛠️ 필수 도구</h3>
            <div class="intro-grid">
                <div class="intro-card">
                    <h4>Android 개발 환경</h4>
                    <ul>
                        <li><strong>Android Studio</strong>: 공식 IDE</li>
                        <li><strong>ADB</strong>: 디바이스 제어 도구</li>
                        <li><strong>Logcat</strong>: 실시간 로그 뷰어</li>
                        <li><strong>Scrcpy</strong>: 화면 미러링</li>
                    </ul>
                </div>
                <div class="intro-card">
                    <h4>iOS 개발 환경</h4>
                    <ul>
                        <li><strong>Xcode</strong>: 공식 IDE</li>
                        <li><strong>Simulator</strong>: iOS 시뮬레이터</li>
                        <li><strong>Console.app</strong>: 로그 분석 도구</li>
                        <li><strong>Instruments</strong>: 성능 프로파일링</li>
                    </ul>
                </div>
                <div class="intro-card">
                    <h4>테스트 관리 도구</h4>
                    <ul>
                        <li><strong>JIRA</strong>: 이슈 트래킹</li>
                        <li><strong>TestRail</strong>: 테스트 케이스 관리</li>
                        <li><strong>Confluence</strong>: 문서화</li>
                        <li><strong>Slack</strong>: 커뮤니케이션</li>
                    </ul>
                </div>
                <div class="intro-card">
                    <h4>유틸리티</h4>
                    <ul>
                        <li><strong>Charles Proxy</strong>: 네트워크 모니터링</li>
                        <li><strong>Postman</strong>: API 테스트</li>
                        <li><strong>Git</strong>: 버전 관리</li>
                        <li><strong>VS Code</strong>: 문서 편집</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Learning Roadmap -->
        <div class="content-card">
            <h2>🎯 학습 로드맵</h2>
            <div class="roadmap">
                <pre>
Week 1 (기초)           Week 2 (설계)           Week 3 (발견)           Week 4 (실전)
    │                       │                       │                       │
    ├─ 도구 숙달            ├─ 화면 분해            ├─ 탐색적 테스팅        ├─ CVT 계획
    ├─ UI 분류              ├─ 데이터 흐름          ├─ 재현 가능 보고       ├─ Smoke Test
    ├─ TC 작성              ├─ 조합 테스트          ├─ 트리아지             ├─ E2E 실행
    ├─ 버그 보고            ├─ E2E 설계             ├─ 리그레션             ├─ 결함 처리
    └─ Mini Project         └─ 테스트 문서          └─ 버그 포트폴리오      └─ 최종 리포트
         │                       │                       │                       │
         └───────────────────────┴───────────────────────┴───────────────────────┘
                               ✅ QA 엔지니어 기본 역량 완성
                </pre>
            </div>
        </div>

        <!-- Checklist -->
        <div class="content-card">
            <h2>✅ 학습 체크리스트</h2>
            <p style="font-size: 1.1em; margin-bottom: 20px;">교육 과정을 진행하면서 아래 항목을 체크하세요:</p>

            <div class="checklist-section">
                <div class="checklist-category">
                    <h3>🔰 기본 역량</h3>
                    <ul>
                        <li>Android/iOS 디바이스를 개발 환경에 연결할 수 있다</li>
                        <li>ADB 명령어를 사용하여 로그를 수집할 수 있다</li>
                        <li>UI 컴포넌트를 6가지 타입으로 분류할 수 있다</li>
                        <li>테스트 케이스를 작성하고 실행할 수 있다</li>
                        <li>재현 가능한 버그 리포트를 작성할 수 있다</li>
                    </ul>
                </div>

                <div class="checklist-category">
                    <h3>📊 중급 역량</h3>
                    <ul>
                        <li>화면 라우팅 다이어그램을 작성할 수 있다</li>
                        <li>데이터 흐름을 추적하고 문제를 발견할 수 있다</li>
                        <li>조합 테스트를 설계할 수 있다 (Pairwise)</li>
                        <li>E2E 시나리오를 사용자 여정 기반으로 작성할 수 있다</li>
                        <li>Severity와 Priority를 정확히 구분할 수 있다</li>
                    </ul>
                </div>

                <div class="checklist-category">
                    <h3>🚀 고급 역량</h3>
                    <ul>
                        <li>탐색적 테스팅 Charter를 작성하고 실행할 수 있다</li>
                        <li>버그 트리아지 회의를 진행할 수 있다</li>
                        <li>리그레션 테스트 전략을 수립할 수 있다</li>
                        <li>CVT 계획을 수립하고 실행할 수 있다</li>
                        <li>Go/No-Go 결정을 위한 리포트를 작성할 수 있다</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Learning Tips -->
        <div class="content-card">
            <h2>💡 학습 팁</h2>
            <div class="tip-grid">
                <div class="tip-card">
                    <h3>📝 효과적인 학습 방법</h3>
                    <ol>
                        <li><strong>매일 실습</strong>: 이론만 읽지 말고 반드시 실제 앱으로 실습</li>
                        <li><strong>산출물 작성</strong>: 모든 실습 결과를 문서화</li>
                        <li><strong>질문 기록</strong>: 이해 안 되는 부분은 메모 후 멘토에게 질문</li>
                        <li><strong>복습</strong>: 주말에 한 주 학습 내용 복습</li>
                        <li><strong>포트폴리오</strong>: 4주 후 최종 결과물을 정리하여 보관</li>
                    </ol>
                </div>

                <div class="tip-card">
                    <h3>⚠️ 주의사항</h3>
                    <ul style="list-style: none; padding-left: 0;">
                        <li style="padding: 5px 0;">❌ 이론만 공부하고 실습 생략하지 않기</li>
                        <li style="padding: 5px 0;">❌ 산출물 대충 작성하지 않기</li>
                        <li style="padding: 5px 0;">❌ 막히는 부분을 혼자 고민만 하지 않기</li>
                        <li style="padding: 5px 0;">❌ 하루 학습량을 미루지 않기</li>
                        <li style="padding: 5px 0;">❌ 버그 리포트를 애매하게 작성하지 않기</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Support & Contact -->
        <div class="content-card">
            <h2>📞 지원 및 문의</h2>
            <div class="contact-section">
                <h3>🙋‍♂️ 질문이 있으신가요?</h3>
                <div class="contact-grid">
                    <div class="contact-item">
                        <strong>멘토 문의</strong><br>
                        각 주차별 담당 멘토에게 Slack DM
                    </div>
                    <div class="contact-item">
                        <strong>기술 지원</strong><br>
                        #qa-training 채널
                    </div>
                    <div class="contact-item">
                        <strong>산출물 피드백</strong><br>
                        매주 금요일 1:1 리뷰
                    </div>
                </div>

                <h3 style="margin-top: 30px;">📊 진도 관리</h3>
                <div class="contact-grid">
                    <div class="contact-item">
                        <strong>일일 체크인</strong><br>
                        매일 오전 학습 계획 공유
                    </div>
                    <div class="contact-item">
                        <strong>주간 리뷰</strong><br>
                        매주 금요일 산출물 제출 및 피드백
                    </div>
                    <div class="contact-item">
                        <strong>최종 평가</strong><br>
                        Week 4 종료 후 최종 CVT 리포트 평가
                    </div>
                </div>
            </div>
        </div>

        <!-- Completion Criteria -->
        <div class="content-card">
            <h2>🎓 수료 기준</h2>
            <p style="font-size: 1.1em; margin-bottom: 20px;">
                아래 조건을 모두 충족하면 <strong>CVT QA 엔지니어 교육 과정 수료증</strong>이 발급됩니다:
            </p>

            <div style="background: #f0fdf4; border-left: 4px solid #10b981; padding: 25px; border-radius: 8px; margin-bottom: 20px;">
                <h3 style="color: #10b981; margin-top: 0;">✅ 필수 조건</h3>
                <ol style="margin-left: 20px;">
                    <li style="margin: 10px 0;"><strong>출석률</strong>: 80% 이상 (16일 이상 참여)</li>
                    <li style="margin: 10px 0;"><strong>산출물 제출</strong>: 주간 Mini-Project 4개 모두 제출</li>
                    <li style="margin: 10px 0;"><strong>최종 과제</strong>: Week 4 CVT 리포트 제출 및 통과 (70점 이상)</li>
                    <li style="margin: 10px 0;"><strong>역량 평가</strong>: 기본 역량 체크리스트 80% 이상 달성</li>
                </ol>
            </div>

            <div style="background: #fef3c7; border-left: 4px solid #f59e0b; padding: 25px; border-radius: 8px;">
                <h3 style="color: #d97706; margin-top: 0;">🏆 우수 수료자 (90점 이상)</h3>
                <ul style="margin-left: 20px;">
                    <li style="margin: 10px 0;">사내 QA 블로그 게시 기회</li>
                    <li style="margin: 10px 0;">차기 교육 과정 멘토 자격</li>
                    <li style="margin: 10px 0;">추천 이력서 작성 지원</li>
                </ul>
            </div>
        </div>

        <!-- License -->
        <div class="content-card">
            <h2>📜 라이선스</h2>
            <p style="font-size: 1.1em; margin-bottom: 20px;">
                본 교육 자료는 <strong>사내 교육 목적으로만</strong> 사용 가능합니다.
            </p>

            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
                <div style="background: #dcfce7; padding: 20px; border-radius: 8px;">
                    <h3 style="color: #10b981; margin-top: 0;">✅ 허용 사항</h3>
                    <ul>
                        <li>사내 공유 및 복사 허용</li>
                        <li>개인 학습 및 복습 허용</li>
                    </ul>
                </div>
                <div style="background: #fee2e2; padding: 20px; border-radius: 8px;">
                    <h3 style="color: #dc2626; margin-top: 0;">❌ 금지 사항</h3>
                    <ul>
                        <li>외부 유출 금지</li>
                        <li>상업적 사용 금지</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Footer -->
        <div class="footer">
            <h3>⭐ 함께 성장하는 QA 엔지니어가 되어봅시다!</h3>
            <p style="margin: 20px 0; color: #666;">Made with ❤️ for CVT QA Engineers</p>
            
            <div class="footer-links">
                <a href="mailto:qa-training@company.com">📧 Contact</a>
                <a href="https://wiki.company.com/qa">📚 More Resources</a>
                <a href="https://company.slack.com/qa-training">💬 Join Slack</a>
            </div>
        </div>
    </div>
</body>
</html>
