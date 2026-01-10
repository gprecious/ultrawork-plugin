# Ultrawork Plugin Marketplace

Sisyphus/Ultrawork 패턴 기반 Claude Code 병렬 에이전트 오케스트레이션 플러그인 마켓플레이스.

## 설치

```bash
# 마켓플레이스 추가
claude plugin marketplace add gprecious/ultrawork-plugin

# 플러그인 설치
claude plugin install ultrawork
```

## 의존성

ultrawork 플러그인을 사용하려면 다음 플러그인들이 **반드시** 활성화되어 있어야 합니다:

```bash
# 필수 플러그인
claude plugin install code-simplifier  # 코드 단순화 검증
claude plugin install code-reviewer    # 버그/보안 코드 리뷰
```

권장 플러그인:
- `context7` - 공식 라이브러리 문서 검색
- `playwright` - 웹 자동화 테스트
- `greptile` - PR 분석
- `figma` - UI/UX 디자인 작업

## 포함된 플러그인

- **ultrawork**: 병렬 에이전트 실행, 모든 외부 도구 총동원, 완료 강제 모드

자세한 내용은 [plugins/ultrawork/README.md](plugins/ultrawork/README.md)를 참조하세요.
