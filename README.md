다운로드 및 설치: QMK_MSYS.exe

QMK MSYS에서 다음 실행

git clone -b gk61_pro_ds https://github.com/NaturalZh/qmk_firmware07072023.git gk61_pro_src

qmk setup

cd gk61_pro_src

make git-submodule

다음 파일 편집 후 저장: ./keyboards/skyloong/gk61/pro_ds/keyboard.json
(편집된 최종본: 이 repository에 있는 keyboard.json)

qmk compile -kb skyloong/gk61/pro_ds -km default

다운로드 및 실행: qmk_toolbox.exe

프로그램 실행 창이 뜨면 qmk 컴파일후 gk61_pro_ds에 생성된 bin파일을 선택 후
esc 키 누른채로 키보드 연결
키보드 (STM32 DFU device) 연결 되었다는 메시지 (노란색) 뜨면 flash 버튼 누름
Flash complete 메시지 (노란색) 뜨면 커스텀 펌웨어 굽기 성공

-----------------------------------------------------------------------------

gk61qmk&via_ds.json : http://usevia.app 사이트에서 키보드 인식시키기 위한 파일
skyloong_gk61_pro_ds.layout.json : http://usevia.app 사이트에서 키보드 인식후 저장된 키보드 레이아웃을 불러오기용 파일
keyboard.json : qmk로 커스텀 키보드 펌웨어 제작을 위한 키보드 설정 파일

