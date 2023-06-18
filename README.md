# koreainvestment-assignment

프로젝트 요구사항:
주요 기능:
주소 정보 분석 및 반환: 수기로 작성된 주소 데이터를 분석하여 실제로 존재하는 주소들 중에서 가장 근접한 주소 정보를 반환합니다. 반환된 주소 정보는 모델 객체 또는 JSON 형태가 됩니다.

주소 정보 객체(ServiceOutput) 상세:
주소 정보 객체는 다음과 같은 정보를 포함합니다:

apiSuccess: 카카오API 사용 여부를 나타내는 불리언 값입니다.

validLevel: 주소 검증 단계를 나타내는 문자열입니다.
  "3" : 사용자가 작성한 정보로 주소를 찾고 카카오 API로 검증
  "2" : 사용자가 작성한 정보를 파싱해서 주소를 찾고 카카오 API로 검증
  "1" : 파싱한 정보만 사용해서 주소를 찾거나 검증 되지 않은 주소 정보

errMsg: 에러 메시지를 나타내는 문자열입니다.

address_name: 전체 도로명 주소

region_1depth_name: 지역명1

region_2depth_name: 지역명2

region_3depth_name: 지역명3

road_name: 도로명

underground_yn: 지하 여부. Y 또는 N으로 표시

main_building_no: 건물 본번

sub_building_no: 건물 부번. 없을 경우 빈 문자열("") 반환

building_name: 건물 이름

zone_no: 우편번호(5자리)

x: X 좌표값. 경위도인 경우 경도(longitude)

y: Y 좌표값. 경위도인 경우 위도(latitude)
