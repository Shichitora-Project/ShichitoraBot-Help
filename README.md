# 七虎なるくんヘルプ

荒らし対策ボット「七虎なるくん」のヘルプです。

開発者も使いこなせてないのですべては書いていません。

ここにないもので何か知りたいことがあれば[お問い合わせ](https://www.shichitora.dev/contact)からヘルプの追加をリクエストしてみてください。

---

## 目次

| タイトル | 説明 |
|---------|------|
| [荒らし対策ルール一覧](#荒らし対策ルール一覧) | 荒らし対策のルールとその機能について |

---

## 荒らし対策ルール一覧

| 名前 | 内部名 | 機能詳細 | カスタム可能な項目 | カテゴリ内部名 |
|------|-------|---------|-------------------|---------------|
| 招待リンク | `invite_link` | Discord招待リンクを検出します。特殊なリンクや独自ドメインリダイレクトも対応しています。 | なし | `link` |
| 逆さ招待リンク | `reverse_invite_link` | 逆文字を利用した疑似招待リンクを検知します。 | なし | `link` |
| ログインリンク | `login_link` | ローカル認証のリンクを検知します。 | なし | `link` |
| アプリ招待リンク | `app_invite_link` | アプリで開く招待リンクを検知します。 | なし | `link` |
| サーバー発見リンク | `discovery_invite_link` | 発見に登録されているサーバーへのリンクを検知します。 | なし | `link` |
| 特殊文字リンク | `special_word_link` | 特殊文字を利用したリンクを検知します。 | なし | `link` |
| リダイレクトリンク | `redirect_link` | リダイレクトが発生するリンクと短縮リンクとして登録されたリンクを検出します。このルールは今後分割される予定です。 | なし | `link` |
| 短縮リンク | `short_link` | 短縮リンクとして登録されたリンクを検出します。現在は未実装です。 | なし | `link` |
| 改行リンク | `line_link` | 改行含まれているリンク化されたものを検知します。 | なし | `link` |
| エンコードリンク | `encode_link` | エンコードが含まれるリンクを検知します。日本語等がエンコードされたリンクをコピペすると検知されてしまうため推奨していません。 | なし | `link` |
| テンプレリンク | `template_link` | Discordサーバーのテンプレートリンクを検出します。 | なし | `link` |
| ボットの招待 | `bot_invite_link` | ボットを導入できるリンクを検知します。 | なし | `link` |
| 危険サイト | `danger_site` | 危険性のあるリンクを検知します。これはAPIの制限からAIルールの方を推奨しています。 | なし | `link` |
| コマンドリンク | `command_link` | コマンドを招待リンクとして見立てたリンクを検知します。 | なし | `link` |
| マークダウンリンクスパム | `markdown` | マークダウンリンクを使ったスパムを検知します。 | なし | `link` |
| 画像サイト | `image_site` | よくスパムに使われる画像サイトのリンクを検知します。 | なし | `link` |
| ドットリンク | `dot_link` | ピリオドを利用したリンク化されたものを検知します。 | なし | `link` |
| ティックトックライトリンク | `tiktok_lite_link` | TikTok Liteのリンクを検知します。 | なし | `link` |
| Kairun招待リンク | `kairun_invite` | Kairunの招待リンクを検知します。 | なし | `link` |
| 国際化ドメインリンク | `punycode` | 国際化されたリンクを検知します。 | なし | `link` |
| Matrix招待リンク | `matrix_invite` | Matrixの招待リンクを検知します。 | なし | `link` |
| 画像リンクスパム | `image_spam` | 画像リンクを使用した詐欺画像スパムを検知します。 | なし | `link` |
| 超特殊文字 | `super_special_character` | 特殊なUnicode文字を悪用した超特殊文字を削除します。 | なし | `other` |
| 冷笑 | `sneer` | 冷笑を検知します。より高度に検知したい場合はAIルールを用いてください。 | なし | `other` |
| 淫夢語録 | `lewd_dream_words` | 某語録を検知します。より高度に検知したい場合はAIルールを用いてください。 | なし | `other` |
| ボットチャットコマンド | `bot_chat_commands` | ボットのチャットコマンドを検知します。 | なし | `other` |
| 認証トークン | `token` | Discordの内部トークンを検知し削除します。 | なし | `other` |
| ベアラートークン | `bearer_token` | ボットの連携トークンを検知し削除します。 | なし | `other` |
| 全体系メンション | `mention` | Everyone, Here, Gameのメンションを削除します。 | なし | `other` |
| スポイラースパム | `spoiler_spam` | スポイラーを多用した処理落ちを狙ったスパムを削除します。 | なし | `other` |
| 処理落ちスパム | `serious_spam` | 処理落ちを狙ったスパムを削除します。 | なし | `other` |
| 海外の迷惑スパム | `christ_spam` | なんかよくわかんない海外のアレを消します。 | なし | `other` |
| 空白スパム | `blank_spam` | 空白だけのメッセージを削除します。 | なし | `other` |
| メールアドレス | `mail` | メールアドレスと思われるものを削除します。 | なし | `other` |
| 電話番号 | `phone` | 電話番号と思われるものを削除します。 | なし | `other` |
| UUID | `uuid` | UUIDを検知します。 | なし | `other` |
| 公式ダイスロール | `roll_dice` | ダイスロール機能を検知します。 | なし | `other` |
| 文字装飾スパム | `zalgo` | Zalgoを使用したスパムを削除します。 | なし | `other` |
| 過激なコンテンツ | `nsfw_content` | 過激なコンテンツを削除します。より高度に検知したい場合はAIルールを用いてください。 | なし | `other` |
| 位置情報の含まれる画像 | `exif_image` | 位置情報が含まれる画像の場合削除します。 | なし | `image` |
| クラッシュGIF対策 | `crash_gif` | クラッシュGIFを検知します。 | なし | `image` |
| フラッシュGIF対策 | `flash_gif` | フラッシュGIFを検知します。 | なし | `image` |
| フラッシュ動画対策 | `flash_video` | フラッシュ動画を検知します。 | なし | `image` |
| 工口画像対策 | `nsfw_image` | 不健全な画像を検知します。 | なし | `image` |
| 工口動画対策 | `nsfw_video` | 不健全な動画を検知します。 | なし | `image` |
| 工口GIF対策 | `nsfw_gif` | 不健全なGIFを検知します。 | なし | `image` |
| Steam詐欺スパム | `steam` | スチーム詐欺を検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| 間違えて通報した | `mistaken_report` | 間違えて通報したという手法の詐欺を検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| アカウント乗っ取り | `account_scam` | アカウント乗っ取りを行う詐欺を検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| 出会い厨対策 | `dating_sexual_inducement` | 出会い厨を消します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| 闇バイト対策 | `dark_job_money` | 闇バイトの可能性があるメッセージを削除します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| 無料ニトロ詐欺対策 | `nitro_free_gift` | 無料Nitro詐欺を検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| シード要求詐欺対策 | `seed_wallet_crypto` | 金銭をだまし取る詐欺を検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| ロマンス詐欺対策 | `romance_money_hybrid` | 結婚詐欺などを検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| 偽認証サポート対策 | `fake_support_verify` | 公式と偽って認証情報を得る詐欺を削除します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| ゲームテスト詐欺対策 | `game_test_malware` | ゲームテストと称したマルウェア配布の可能性があるメッセージを削除します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| QRログイン詐欺対策 | `qr_code_phish` | ローカル認証を悪用した詐欺を検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| 偽電話詐欺対策 | `fake_voice_call` | 音声通話を装った不正なリンクやスパムを検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| 偽求人対策 | `recruitment_job_scam` | 実在しない企業の求人を装ったフィッシングを検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| 乗っ取り招待送信対策 | `hijacked_invite_link` | 乗っ取られたアカウントから一斉送信される招待リンクを検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| AI偽人物対策 | `ai_romance_deepfake` | AI生成による偽の人物画像を使った詐欺や誘導をブロックします。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| 偽認証画面対策 | `clickfix_powershell` | 「認証に失敗しました」等と表示させスクリプトを実行させる詐欺を検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| PayPay詐欺対策 | `paypay_scam` | PayPay送金を要求するスパムや詐欺メッセージを検知します。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| 偽ボット導入詐欺対策 | `fake_bot_scam` | 有名なBotに偽装して不正な権限を要求する導入詐欺をブロックします。これらは誤検知の可能性があり、AI検知への移行が推奨されています。 | なし | `scam` |
| ボイチャステータスチェック | `voice_status_check` | 有効化されているルールに応じて名前を検閲します。 | なし | `name` |
| ユーザー名チェック | `username_check` | 有効化されているルールに応じて名前を検閲します。 | なし | `name` |
| スレッド名チェック | `thread_name_check` | 有効化されているルールに応じて名前を検閲します。 | なし | `name` |
| チャンネル名チェック | `channel_name_check` | 有効化されているルールに応じて名前を検閲します。 | なし | `name` |
| ロール名チェック | `role_name_check` | 有効化されているルールに応じて名前を検閲します。 | なし | `name` |
| イベント名・説明チェック | `event_name_description_check` | 有効化されているルールに応じて名前を検閲します。 | なし | `name` |
| リアクションスパム | `reaction_spam` | メッセージへの大量のリアクションを検知します。 | `timeframe`, `limit` | `special` |
| リアクションレイド | `reaction_raid` | 複数人によるメッセージへの大量のリアクションを検知します。 | `timeframe`, `reactionLimit` | `special` |
| スレッド作成スパム | `thread_create` | スレッドを過度に作成する行為を検知します。 | `timeframe`, `reactLimit` | `special` |
| スレッド更新スパム | `thread_update` | スレッドを過度に更新する行為を検知します。 | `timeframe`, `threadLimit` | `special` |
| スレッド削除スパム | `thread_delete` | スレッドを過度に削除する行為を検知します。 | `timeframe`, `threadLimit` | `special` |
| イベント作成スパム | `event_create` | イベントを過度に作成する行為を検知します。 | `timeframe`, `eventLimit` | `special` |
| イベント更新スパム | `event_update` | イベントを過度に更新する行為を検知します。 | `timeframe`, `eventLimit` | `special` |
| イベント削除スパム | `event_delete` | イベントを過度に削除する行為を検知します。 | `timeframe`, `eventLimit` | `special` |
| 招待リンク作成スパム | `invite_create_spam` | 招待リンクを過度に作成する行為を検知します。 | `timeframe`, `inviteLimit` | `special` |
| サウンドボードスパム | `soundboard_spam` | サウンドボードを過剰に使用する行為を検知します。 | `timeframe`, `soundLimit` | `special` |
| ウェブカメラ共有 | `self_video` | ウェブカメラ等を使用したリアルの画面共有を検知します。 | なし | `special` |
| メッセージ更新制限 | `message_update` | 過度なメッセージ更新を検知します。 | `timeframe`, `messageLimit` | `special` |
| サーバー参加レイド対策 | `member_join` | 過度なサーバー参加を検知します。 | `timeframe`, `joinLimit` | `special` |
| VC参加レイド対策 | `vc_raid` | 過度なボイスチャットへの参加を検知します。 | `timeframe`, `memberLimit` | `special` |
| ピン留めスパム対策 | `pin_spam` | 過度なピン留めを検知します。 | `timeframe`, `pinLimit` | `special` |
| スパム | `spam` | 過度なメッセージ送信を検知します。 | `timeframe`, `messageLimit` | `message` |
| レイド | `raid` | 複数人による過度なメッセージ送信を検知します。 | `timeframe` | `message` |
| 重複メッセージ | `duplicate` | 前回送信したメッセージと似通っているメッセージを検知します。 | `timeframe`, `similarity` | `message` |
| 詐欺画像スパム | `scam_image` | AIを用いて詐欺画像を検知します。 | `similarityThreshold`, `textSimilarityThreshold` | `message` |
| メンションスパム | `mention_spam` | メンションを過度に行う行為を検知します。 | `timeframe`, `mentionLimit` | `message` |
| メンション制限 | `mention_restrict` | 特定のメンションしか受け付けないようにします。 | 特殊 | `message` |
| 返信スパム | `reply_spam` | 過度な返信を検知します。 | `timeframe`, `replyLimit` | `message` |
| 詐欺スレッド対策 | `scam_thread` | 詐欺スレッドを検知します。 | `titleMinLength`, `messageMinLength` | `message` |
| 長文制限 | `long_message` | 過度な長文を検知します。 | `messageLimit` | `message` |
| 改行制限 | `too_many_line` | 過度な改行を検知します。 | `timeframe`, `lineLimit` | `message` |
| 投票制限 | `too_poll` | 過度な投票の送信を検知します。 | `timeframe`, `pollLimit` | `message` |
| 同じ文字のリピート | `character_repeats` | 過度に同じ文字を連続して使っているメッセージを検知します。 | `timeframe`, `repeatLimit` | `message` |
| 特定文字スパム | `specific_char_spam` | 特定の文字の使用回数を制限します。 | 特殊 | `message` |
| 画像数制限 | `too_many_images` | 過度な画像の使用を検知します。 | `timeframe`, `imageLimit` | `message` |
| 絵文字数制限 | `too_emoji` | 過度な絵文字の使用を検知します。 | `timeframe`, `emojiLimit` | `message` |
| リンク数制限 | `too_link` | 過度なリンクの使用を検知します。 | `timeframe`, `linkLimit` | `message` |
| 埋め込み数制限 | `too_embed` | 過度な埋め込みの使用を検知します。 | `timeframe`, `embedLimit` | `message` |
| スタンプ数制限 | `stamp_spam` | 過度なスタンプの使用を検知します。 | `timeframe`, `stampLimit` | `message` |
| Markdown装飾スパム | `markdown_spam` | 過度なマークダウンの使用を検知します。 | `ratio` | `message` |
| チャンネル作成 | `channel_create` | チャンネルを過度に作成する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| チャンネル更新 | `channel_update` | チャンネルを過度に更新する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| チャンネル削除 | `channel_delete` | チャンネルを過度に削除する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| ロール作成 | `role_create` | ロールを過度に作成する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| ロール更新 | `role_update` | ロールを過度に更新する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| ロール削除 | `role_delete` | ロールを過度に削除する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| ウェブフック作成 | `webhook_create` | ウェブフックを過度に作成する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| ウェブフック更新 | `webhook_update` | ウェブフックを過度に更新する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| ウェブフック削除 | `webhook_delete` | ウェブフックを過度に削除する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| メンバーBAN | `member_ban_add` | BANを過度に執行する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| メンバーKick | `member_kick` | Kickを過度に執行する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| メンバーTimeOut | `member_timeout` | タイムアウトを過度に執行する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| 絵文字作成 | `emoji_create` | 絵文字を過度に作成する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| 絵文字更新 | `emoji_update` | 絵文字を過度に更新する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| 絵文字削除 | `emoji_delete` | 絵文字を過度に削除する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| ステッカー作成 | `sticker_create` | ステッカーを過度に作成する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| ステッカー更新 | `sticker_update` | ステッカーを過度に更新する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| ステッカー削除 | `sticker_delete` | ステッカーを過度に削除する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| サウンドボード作成 | `soundboard_create` | サウンドボードを過度に作成する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| サウンドボード更新 | `soundboard_update` | サウンドボードを過度に更新する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| サウンドボード削除 | `soundboard_delete` | サウンドボードを過度に削除する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| オートモッドルール更新 | `automod_update` | AutoModルールを過度に更新する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| オートモッドルール削除 | `automod_delete` | AutoModルールを過度に削除する行為を検知します。 | `timeframe`, `nukeLimit` | `nuke` |
| リンク用の文字列検知補正 | `char_correction_ai` | リンク向けに文字列を補正します。 | なし | `ai` |
| スパムが送信したメッセージ | `spam_message_ai` | スパムメッセージかAIが判断します。 | なし | `ai` |
| 詐欺メッセージ | `scam_message_ai` | 詐欺メッセージかAIが判断します。 | なし | `ai` |
| 迷惑メッセージ | `trouble_message_ai` | 迷惑メッセージかAIが判断します。 | なし | `ai` |
| 嫌なネットミームが含まれる | `unpleasant_internet_meme_ai` | 嫌なネットミームが含まれるかAIが判断します。 | なし | `ai` |
| 不適切なコンテンツが含まれる | `inappropriate_content_ai` | 不適切なコンテンツが含まれるかAIが判断します。 | なし | `ai` |
| 犯罪や危険性のあるコンテンツ | `danger_content_ai` | 犯罪や危険性のあるコンテンツかAIが判断します。 | なし | `ai` |
| 個人情報が含まれるコンテンツ | `private_info_ai` | 個人情報が含まれるコンテンツかAIが判断します。 | なし | `ai` |
| カスタムルール | `custom` | 自分だけのカスタムルールを作成します。 | 特殊 | `custom` |
| 招待リンク作成チャンネル制限 | `invite_restrict` | 招待リンクを作成できるチャンネルを制限します。このルールは、ルールホワイトリストに対応していますが、ルールホワイトリストを設定することができません。 | 特殊 | なし |
| SNSリンクの発信者の制限 | `sns_restrict` | SNSリンクの発信者の制限します。このルールは、ルールホワイトリストに対応していますが、ルールホワイトリストを設定することができません。 | 特殊 | なし |
