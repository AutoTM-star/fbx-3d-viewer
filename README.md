# FBX 3D 뷰어

Revit에서 내보낸 FBX 파일을 브라우저에서 바로 3D로 확인하는 단일 HTML 뷰어입니다.

## 사용법
1. `index.html`을 브라우저(Chrome/Edge)로 엽니다. (인터넷 연결 필요 — three.js를 CDN에서 불러옴)
2. 왼쪽 칸에 FBX 파일을 끌어다 놓거나 클릭해서 선택합니다. 여러 개 가능.
3. 목록에서 파일을 누르면 3D 형상과 외형 크기(W×D×H, mm)가 표시됩니다.

- 마우스: 왼쪽 드래그 회전 · 오른쪽 드래그 이동 · 휠 확대
- 시점: 3D / 정면 / 평면 / 우측
- 옵션: 와이어프레임, 모서리선, 단색 재질, 전체 나란히 보기
- 지원 형식: FBX 바이너리·텍스트(ASCII), OBJ·STL(mm 가정), GLB
- FBX의 위쪽 축(Y/Z)과 단위(UnitScaleFactor)를 읽어 자동 보정, 단위는 화면에서 직접 변경 가능
- 비표준 텍스트 FBX(한 줄 블록, 쉼표 뒤 공백) 자동 보정
- Revit FBX 재질 색 표시: Revit은 재질을 표준 Material이 아닌 Autodesk 자산(ADSKAssetReferences)으로 저장 → 뷰어가 직접 읽어 색 적용
- 프로젝트에서 내보낸 FBX의 레벨 표식 자동 숨김

파일은 서버로 전송되지 않고 브라우저 안에서만 처리됩니다.

## samples/
Revit 2027에서 제작·내보낸 예제 FBX

| 파일 | 내용 |
|---|---|
| 01 | 실내기 1WAY TT + 판넬 PFP-VT2CW |
| 02 | 실내기 1WAY TU + 판넬 PFP-VU2SW |
| 03 | 실내기 1WAY TG + 판넬 PFP-VG2SW |
| 04 | 실외기 MULTI V S U30A (RPUQ0405) |
| 05 | 실외기 MULTI V S U36A (RPUQ0506/0606) |
| 06~08 | 스프링클러 헤드 |
