# 納品素材（原本）

2026-09-28 納品分（Google Drive 経由）。`tools/asset_prep` の入力であり、ゲームからは直接参照しない（`.gdignore` により Godot の取り込み・書き出しの対象外）。
シナリオ原稿として `scenario_test` も同梱されていたが、空ファイル（0 バイト）だったため取り込んでいない。

| ファイル | 納品時のファイル名 |
| --- | --- |
| `bg_entrance.png` | 背景自動ドア.png |
| `bg_izakaya.png` | 背景居酒屋.png |
| `bg_keiko_room.png` | 背景けいこの部屋.png |
| `bg_science_room.png` | 背景理工学部.png |
| `conversation_fast_forward.png` | 会話早送り.png |
| `conversation_skip.png` | 会話SKIP.png |
| `keiko_closeup.png` | ケイコアップ.png |
| `keiko_disgust.png` | ケイコドン引き.png |
| `keiko_normal.png` | ケイコ真顔.png |
| `keiko_smile.png` | ケイコ笑う.png |
| `keiko_smug.png` | ケイコナメてる.png |
| `loading.png` | ロード.png |
| `message_keiko.png` | 会話ケイコ.png |
| `message_nega.png` | 会話ネガ.png |
| `message_student_commerce.png` | 会話商学部学生.png |
| `message_student_science.png` | 会話理工学部学生png.png |
| `place_entrance.png` | 会話6号館エントランス.png |
| `place_izakaya.png` | 会話居酒屋.png |
| `place_science_room.png` | 会話理工学部教室.png |
| `title_background.png` | タイトル画像.png |
| `title_composite.png` | タイトル完成形png.png |
| `title_continue.png` | タイトル続きからpng.png |
| `title_logo.png` | タイトルネガケイコ.png |
| `title_start.png` | タイトル初めから.png |
| `battle_cue_swing.png` | 振り上げ1.PNG（2026-10-01。ケイコが手を振り上げる絵。UI の見本の枠・会話窓・ゲージ・四隅の飾り入りの横長 1920×1080。パート B の一枚絵の土台） |
| `app_icon.png` | 無題156_20261001150740.png（2026-10-01。アプリアイコン。2048×2048、不透明。ゲームでは res/images/art/app_icon.png に 1024×1024・透過なしで縮小して使う） |
| `bg_karaoke_room.png` | 無題158_20261001152025.png（2026-10-01。カラオケ個室の室内。立った視点・座った視点で共通） |

## 2026-10-11 納品分（`new_assets/`）

| ファイル | 納品時のファイル名 | 内容 |
| --- | --- | --- |
| `explore_karaoke_with_items.png` | 無題172_20261011162743.PNG | 探索の部屋（カラオケ個室・POV）。アイテムが置かれた状態（2048×2048） |
| `explore_karaoke_empty.png` | 無題172_20261011200027.png | 同じ部屋からアイテムを除いた状態（探索の背景になる） |
| `item_menu_stand.png` | 無題172_20261011163053.PNG | アイテム単体：メニュー立て（白地） |
| `item_mic.png` | 無題172_20261011163416.PNG | アイテム単体：マイク（白地） |
| `item_glass.png` | 無題172_20261011163819.PNG | アイテム単体：グラス（白地） |
| `item_hanger.png` | 無題172_20261011164023.PNG | アイテム単体：ハンガー（白地） |
| `item_denmoku.png` | 無題172_20261011164352.PNG | アイテム単体：デンモク（カラオケのリモコン。白地） |

- 漫画のページ `p1.png`〜`p3.png`（1240×1754）は `res/comic/chapter_01/` にそのまま置いた（ゲームが直接読む）。
- 探索の背景・部屋の中のアイテム・アイコンは `tools/asset_prep/derive_explore_items.py` で `res/images/art/` に作る。

## 2026-10-12 納品分（`new_assets/`）

パート B の「掴む」差分。振り上げ1 と同じ構図・同じ位置（1920×1080、地は透過）。手が物を握る形に描かれていて、道具は描かれていない。顔は振り上げ1 と同じで、口だけ違う。

| ファイル | 納品時のファイル名 | 内容 |
| --- | --- | --- |
| `spank_grip_low.png` | 無題122_20261012133254.png | 胸の前で握る（道具を見せる）。口は歯の見える笑み |
| `spank_grip_mid.png` | 無題116_20261012140833.png | 肩の高さで握る（構える）。口は少し開く |
| `spank_grip_high.png` | 無題120_20261012140443.png | 頭の上で握る（振り上げる）。口は開く |

- 道具を手に組み込んだ絵は `tools/asset_prep/derive_spank_scene.py` → `compose_spank_scene.py` で `res/images/art/` に作る（`docs/part_b.md`）。


## 2026-10-26 受領分（Google Drive「Keiko/Assets/まんが」）

最終章の漫画 4 ページ。ページごとにレイヤー分けされた透過 PNG（各 1240×1754、A4・150dpi）。重ね順は 背景 → 絵 → 枠 → 言葉（背景は 4 ページだけ）。
原本のレイヤーは `res/comic/finale/layers/` に置いた（名前は ASCII に直した。`.gdignore` で Godot の取り込みの対象外）。

| ファイル | 受領時のファイル名 |
| --- | --- |
| `p1_frame.png` `p1_art.png` `p1_words.png` | 1枠.png 1絵.png 1言葉.png |
| `p2_frame.png` `p2_art.png` `p2_words.png` | 2枠.png 2絵.png 2言葉.png |
| `p3_frame.png` `p3_art.png` `p3_words.png` | 3枠.png 3絵.png 3言葉.png |
| `p4_background.png` `p4_frame.png` `p4_art.png` `p4_words.png` | 4背景.png 4枠.png 4絵.png 4言葉.png |

- コマの画像（`res/comic/finale/panels/`）は `old/tools/asset_prep/slice_layered_comic.py`（定義 `comic_panels/finale.json`）で作る。
- p4 のスマホのアラーム（「幼稚園 おむかえ」）は絵のレイヤーに手描き。ゲームでは使わず、届いた大写し（下）に置き換える（`comic_panels/finale.json` の `delivered`）。
- 書き換わるコマ（スマホのアラームの大写し）：2026-10-30 に受け取った `true.png`（「9月30日 木曜日 15:30 保育園おむかえ」）と `fake.png`（同じ構図で「サークル飲み」）。どちらも 1240×1754 で、`res/comic/finale/layers/p4_12_truth_source.png`・`p4_12_fake_source.png` に置き、描かれた範囲（270, 874）〜（991, 1385）を `panels/p4_12.png`（真相）・`panels/p4_12_rewritten.png`（書き換え後）に切り出す（`slice_layered_comic.py` の `delivered`）。
- PV（v21）の前半の漫画：2026-10-31 に受け取った 4 ページ（`無題160_20261029222314.jpg`・`無題161_…222843.jpg`・`無題177_…223734.jpg`・`無題179_…224424.jpg`、1240×1754）。描かれた所で切り抜き、白い地を透明にして `res/comic/chapter_01/pv/pv_opening_01〜04.png` に置く。PV だけで使い、ゲームの漫画には入れていない。
