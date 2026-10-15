# 사진풍 물고기 이미지 사양

Built-in image_gen으로 생성했습니다. 외부 촬영 사진을 사용하지 않았습니다.

## Coastal atlas

Prompt specification: photorealistic freshly caught Korean coastal fish cutouts in 4 columns by 7 rows, head right, whole body strict side profile, soft photographic lighting, visible real overlapping scales and wet mucus, translucent fin rays, species-specific natural coloration, genuinely transparent background, no text or labels, not drawing/painting/vector/plastic. 26 species ordered according to PHOTO_FISH_IDS in game.js.

## Special atlas

Prompt specification: four photorealistic Korean coastal fish in a 2x2 transparent sprite atlas, strict side profile, head right, whole body and fins visible. Upper left Hypodytes rubripinnis (미역치); upper right Siganus fuscescens (독가시치); lower left Tribolodon hakonensis (황어); lower right Chelidonichthys spinosus (성대) with broad blue-green-edged pectoral fins and three free rays. Natural scales, mucus and translucent membranes. No text, hooks, hands or background.

Background extraction edit: preserve exact four fish and positions; remove every blurred background pixel, preserve opaque fish and fine fin rays, true zero-alpha empty background, no gradient or shadow.

원본 PNG는 그대로 저장하며, 코드의 영역 좌표로 각 어종을 표시합니다. 절차적 그림은 이미지 로딩 실패 시 대체로 유지합니다.
