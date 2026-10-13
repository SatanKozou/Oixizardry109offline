# Oixizardry109offline
ファミコン版初代ウィザードリィクローンの作成（最終的には１０９人同時プレイが目標）

今回は、オフライン版（ブラウザ版）

まずは、TypeScript＋React

Vite ＋ React ＋ TypeScript

npm create vite@latest oixizardry109offline -- --template react-ts

npmはNodePackageManager
Viteはビルドツール

とりあえず、
/user/Satan/Documents/MyProjects/oixizardry109offline/


npmで　zustandとdexieとlucide-reactをインストール
$ npm install zustand
$ npm install dexie
$ npm install lucide-react

src/
├── types/          # キャラクター型、アイテム型、モンスター型などの定義 (d.ts)
├── store/          # ゲームの状態管理（セーブ・ロード、バトル状態など）
├── components/     # 共通UI（3D風ダンジョンビュー、ログウィンドウ、ステータス画面）
├── hooks/          # ゲームのロジック（移動処理、ターン制バトルの計算など）
├── data/           # マスターデータ（アイテム一覧、モンスター図鑑、マップデータ）


src/
├── components/純UI ステータスパネル
├── pages/ 
├── features/ 
├── systems/
├── data/
├── hooks/
├── store/
├── types/
├── utils/
└── App.tsx

pages/
├── Title
├── Castle
├── Tavern
├── Shop/TradingPost
├── TrainingGround
├── Dungeon/Maze/World
├── Battle

features/
├── party/
├── battle/
├── dungeon/
├── shop/
├── item/
├── character/

systems/
├── save/
├── rng/
├── event/
└── game/

data/
├── jobs.ts
├── races.ts
├── monsters.ts
├── items.ts
├── spells.ts

types/
├── Character.ts
├── Item.ts
├── Monster.ts
├── Spell.ts

store/状態管理Zustand推奨
├── gameStore.ts
├── partyStore.ts
├── battleStore.ts



v0.1.0 タイトル画面
v0.2.0 キャラ作成
v0.3.0 酒場
v0.4.0 ダンジョン
v0.5.0 戦闘
v1.0.0 オフライン完成

カード例
タイトル画面
酒場画面
訓練場
商店
地下1階マップ
戦闘システム
僧侶呪文
魔法使い呪文
セーブロード


battleLogic.ts
battleStore.ts
battleView.tsx


Phase1 タイトル画面
↓
Phase2 キャラ作成
↓
Phase3 酒場
↓
Phase4 訓練場
↓
Phase5 商店
↓
Phase6 ダンジョン移動
↓
Phase7 戦闘
↓
Phase8 呪文
↓
Phase9 セーブロード
↓
v1.0完成

