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

