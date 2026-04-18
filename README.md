다운로드 및 설치: QMK_MSYS.exe

QMK MSYS에서 다음 실행

git clone -b gk61_pro_ds https://github.com/NaturalZh/qmk_firmware07072023.git gk61_pro_src

qmk setup

cd gk61_pro_src

make git-submodule

다음 파일 편집 후 저장: ./keyboards/skyloong/gk61/pro_ds/keyboard.json
(편집된 최종본: 이 repository에 있는 keyboard.json)

qmk compile -kb skyloong/gk61/pro_ds -km default
