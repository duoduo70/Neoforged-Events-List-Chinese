> [!IMPORTANT]
> 
> Copyright (c) 2024 plasma (duoduo70) 
> 以 CC BY-NC-ND 4.0 协议授予你有限权利
> 
> 基于 NeoForged commit 412c6ab (Minecraft 1.21, 2024/6/24)  
> 
> 为保证翻译的一致性，若您想更改它们，请提交 Pull Request  
> See: https://github.com/duoduo70/Neoforged-Events-List-Chinese
>
> Github 无法正常显示超宽列表，为保证最好的阅读体验，建议前往 https://duoduo70.github.io/Neoforged-Events-List-Chinese/
---

不翻译的专有名词：

- `FML`: Forge 模组载入器
- `Tick`: [游戏刻](https://zh.minecraft.wiki/w/%E5%88%BB#%E6%B8%B8%E6%88%8F%E5%88%BB%E4%B8%8E%E8%AE%A1%E7%AE%97%E9%80%9F%E7%8E%87)
- `FOV`: 视野
- `Container`: GUI 所对应的数据结构
- `Living` 暂且翻译成「活体」，字面意思，有生命值的实体，例如动物和怪物
- `Effects` 有两种意思，一种是字面意思的效果，另一种同其它游戏的 `buff` / `debuff`，需仔细辨别含义
- `Level` 的意思可能是「世界」或「等级」，等级可能是经验等级，亦或者是 `Ticket` 区块加载优先级
- `Ticket` 是一种区块加/卸载器

有些事件的翻译可能有错，因为其实我也不知道它们是干啥的。

你显然只能大概知道这些事件是做什么的，到底符不符合你的需求需要你自己去看它们的代码

关于使用脚本处理本文件：
你只需遵从惯例，`$` 一律转换为 `－`。

---

| 事件名                                        | 短描述                              | 长描述                                                                                                                                                               |
| --------------------------------------------- | ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `ModConfigEvent$Loading`                        | 模组配置事件－加载中               |
| `ModConfigEvent$Reloading`                      | 模组配置事件－重新加载中           |
| `ModConfigEvent$Unloading`                      | 模组配置事件－卸载中               |
| `ModConfigEvent`                                | 模组配置事件                        |
| `FMLClientSetupEvent`                           | FML 客户端设置事件                |
| `FMLCommonSetupEvent`                           | FML 通用设置事件                  |
| `FMLConstructModEvent`                          | FML 构建模组事件                  |
| `FMLDedicatedServerSetupEvent`                  | FML 专用服务器设置事件            |
| `FMLLoadCompleteEvent`                          | FML 加载完成事件                  |
| `InterModEnqueueEvent`                          | 模组间事件队列事件                  |
| `InterModProcessEvent`                          | 模组间处理事件                      |
| `ModLifecycleEvent`                             | 模组生命周期事件                    |
| `ParallelDispatchEvent`                         | 并行调度事件                        |
| `RegisterCapabilitiesEvent`                     | 注册能力事件                        |
| `PlaySoundEvent`                                | 播放声音事件                        |
| `PlaySoundSourceEvent`                          | 播放声音源事件                      |
| `PlayStreamingSourceEvent`                      | 播放流媒体源事件                    |
| `SoundEngineLoadEvent`                          | 声音引擎加载事件                    |
| `SoundEvent$SoundSourceEvent`                   | 声音事件－声音源事件               |
| `SoundEvent`                                    | 声音事件                            |
| `AddSectionGeometryEvent`                       | 添加区段几何事件                    |
| `CalculateDetachedCameraDistanceEvent`          | 计算分离摄像机距离事件              |
| `CalculatePlayerTurnEvent`                      | 计算玩家转向事件                    |
| `ClientChatEvent`                               | 客户端聊天事件                      | 每当客户端要向服务器发送聊天消息或命令时，就会触发                                                                                                                   |
| `ClientChatReceivedEvent$Player`                | 客户端接收聊天事件－玩家           |
| `ClientChatReceivedEvent$System`                | 客户端接收聊天事件－系统           |
| `ClientChatReceivedEvent`                       | 客户端接收聊天事件                  | 收到聊天消息时在客户端上触发。如果取消此事件，则该消息不会显示在聊天消息窗口中                                                                                       |
| `ClientPauseChangeEvent$Post`                   | 客户端暂停改变事件－后置           |
| `ClientPauseChangeEvent$Pre`                    | 客户端暂停改变事件－前置           |
| `ClientPauseChangeEvent`                        | 客户端暂停改变事件                  |
| `ClientPlayerChangeGameTypeEvent`               | 客户端玩家改变游戏类型事件          | 在客户端玩家收到服务器游戏模式更改的通知之前触发                                                                                                                     |
| `ClientPlayerNetworkEvent$Clone`                | 客户端玩家网络事件－克隆           |
| `ClientPlayerNetworkEvent$LoggingIn`            | 客户端玩家网络事件－登录中         |
| `ClientPlayerNetworkEvent$LoggingOut`           | 客户端玩家网络事件－登出中         |
| `ClientPlayerNetworkEvent`                      | 客户端玩家网络事件                  | 客户端玩家连接事件                                                                                                                                                   |
| `ClientTickEvent$Post`                          | 客户端游戏刻事件－后置           |
| `ClientTickEvent$Pre`                           | 客户端游戏刻事件－前置           |
| `ClientTickEvent`                               | 客户端游戏刻事件                  |
| `ComputeFovModifierEvent`                       | 计算 FOV 修改事件                 |
| `ContainerScreenEvent$Render$Background`        | 容器界面事件－渲染－背景  |
| `ContainerScreenEvent$Render$Foreground`        | 容器界面事件－渲染－前景  |
| `ContainerScreenEvent$Render`                   | 容器界面事件－渲染         |
| `ContainerScreenEvent`                          | 容器界面事件                |
| `CustomizeGuiOverlayEvent$BossEventProgress`    | 自定义GUI覆盖事件－Boss 事件进度 |
| `CustomizeGuiOverlayEvent$Chat`                 | 自定义GUI覆盖事件－聊天            |
| `CustomizeGuiOverlayEvent$DebugText`            | 自定义GUI覆盖事件－调试文本        |
| `CustomizeGuiOverlayEvent`                      | 自定义GUI覆盖事件                   |
| `EntityRenderersEvent$AddLayers`                | 实体渲染器事件－添加图层           |
| `EntityRenderersEvent$CreateSkullModels`        | 实体渲染器事件－创建头骨模型       | 提供一个安全的地方来注册头骨块模型（类似那些可以放到地上的怪物的头）                                                                                                 |
| `EntityRenderersEvent$RegisterLayerDefinitions` | 实体渲染器事件－注册图层定义       | 提供一个安全的地方来注册实体渲染器和图层渲染器                                                                                                                       |
| `EntityRenderersEvent$RegisterRenderers`        | 实体渲染器事件－注册渲染器         | 挂钩到 `GameRenderer` 的事件，允许任何功能自定义玩家看到的视觉属性                                                                                                   |
| `EntityRenderersEvent`                          | 实体渲染器事件                      |
| `InputEvent$InteractionKeyMappingTriggered`     | 输入事件－触发交互键映射           | 在键绑定里配置的那种                                                                                                                                                 |
| `InputEvent$Key`                                | 输入事件－击键                     |
| `InputEvent$MouseButton$Post`                   | 输入事件－鼠标按键－后置          |
| `InputEvent$MouseButton$Pre`                    | 输入事件－鼠标按键－前置          |
| `InputEvent$MouseButton`                        | 输入事件－鼠标按键                 |
| `InputEvent$MouseScrollingEvent`                | 输入事件－鼠标滚轮事件             |
| `InputEvent`                                    | 输入事件                            |
| `ModelEvent$BakingCompleted`                    | 模型事件－烘焙完成                 |
| `ModelEvent$ModifyBakingResult`                 | 模型事件－修改烘焙结果             | 用于处理先前在 `ModelEvent$BakingCompleted` 中完成的 [状态 -> 模型] 映射的缓存。这些用例通常源于由于无法使用自定义加载程序或提供的上下文不足而需要对模型进行调整的用户 |
| `ModelEvent$RegisterAdditional`                 | 模型事件－注册附加模型             | 注册不以某种方式与块或项目关联，但在其他上下文中仍然需要的模型                                                                                                       |
| `ModelEvent$RegisterGeometryLoaders`            | 模型事件－注册几何加载器           | 用于自定义模型几何形状                                                                                                                                               |
| `ModelEvent`                                    | 模型事件                            |
| `MovementInputUpdateEvent`                      | 移动输入更新事件                    | 更新玩家移动输入后会触发此事件，处理程序可以自由操纵 `Input` 来取消移动                                                                                                |
| `RecipesUpdatedEvent`                           | 配方更新事件                        | 当 `RecipeManager` 将其所有配方从服务器同步到客户端时（在客户端连接后）触发                                                                                            |
| `RegisterClientCommandsEvent`                   | 注册客户端命令事件                  | 触发以允许模组注册客户端命令                                                                                                                                         |
| `RegisterClientReloadListenersEvent`            | 注册客户端重载监听器事件            | 触发以允许模组在客户端资源管理器上注册重载侦听器，该事件在 `Minecraft` 实例构建期间触发一次                                                                            |
| `RegisterClientTooltipComponentFactoriesEvent`  | 注册客户端提示框组件工厂事件        | 允许用户为其 `TooltipComponent` 类型注册自定义 `ClientTooltipComponent` 工厂                                                                                             |
| `RegisterColorHandlersEvent$Block`              | 注册颜色处理程序事件－方块         |
| `RegisterColorHandlersEvent$ColorResolvers`     | 注册颜色处理程序事件－颜色解析器   |
| `RegisterColorHandlersEvent$Item`               | 注册颜色处理程序事件－物品         |
| `RegisterColorHandlersEvent`                    | 注册颜色处理程序事件                |
| `RegisterDimensionSpecialEffectsEvent`          | 注册维度特效事件                    |
| `RegisterEntitySpectatorShadersEvent`           | 注册实体观察者着色器事件            |
| `RegisterGuiLayersEvent`                        | 注册GUI图层事件                     |
| `RegisterItemDecorationsEvent`                  | 注册物品装饰事件                    |
| `RegisterKeyMappingsEvent`                      | 注册按键映射事件                    |
| `RegisterMenuScreensEvent`                      | 注册菜单界面事件                    |
| `RegisterNamedRenderTypesEvent`                 | 注册命名渲染类型事件                | https://docs.minecraftforge.net/en/latest/rendering/modelextensions/rendertypes/                                                                                     |
| `RegisterParticleProvidersEvent`                | 注册粒子 Provider （创建器）事件  |
| `RegisterPresetEditorsEvent`                    | 注册预设编辑器事件                  |
| `RegisterRecipeBookCategoriesEvent`             | 注册配方书类别事件                  |
| `RegisterRenderBuffersEvent`                    | 注册渲染缓冲区事件                  |
| `RegisterShadersEvent`                          | 注册着色器事件                      |
| `RegisterSpriteSourceTypesEvent`                | 注册精灵源事件                      |
| `RenderArmEvent`                                | 渲染手臂事件                        |
| `RenderBlockScreenEffectEvent`                  | 渲染方块界面效果事件                |
| `RenderFrameEvent$Post`                         | 渲染帧事件－后置                   |
| `RenderFrameEvent$Pre`                          | 渲染帧事件－前置                   |
| `RenderFrameEvent`                              | 渲染帧事件                          |
| `RenderGuiEvent$Post`                           | 渲染 `GUI` 事件－后置              |
| `RenderGuiEvent$Pre`                            | 渲染 `GUI` 事件－前置              |
| `RenderGuiEvent`                                | 渲染 `GUI` 事件                     |
| `RenderGuiLayerEvent$Post`                      | 渲染 `GUI` 层事件－后置            |
| `RenderGuiLayerEvent$Pre`                       | 渲染 `GUI` 层事件－前置            |
| `RenderGuiLayerEvent`                           | 渲染 `GUI` 层事件                   |
| `RenderHandEvent`                               | 渲染手事件                          |
| `RenderHighlightEvent$Block`                    | 渲染高亮事件－方块                 |
| `RenderHighlightEvent$Entity`                   | 渲染高亮事件－实体                 |
| `RenderHighlightEvent`                          | 渲染高亮事件                        |
| `RenderItemInFrameEvent`                        | 每帧渲染物品事件                    |
| `RenderLevelStageEvent$RegisterStageEvent`      | 渲染世界阶段事件－注册阶段事件     |
| `RenderLevelStageEvent`                         | 渲染世界阶段事件                    |
| `RenderLivingEvent$Post`                        | 渲染活体事件－后置                 | 可用于追加渲染一些东西                                                                                                                                               |
| `RenderLivingEvent$Pre`                         | 渲染活体事件－前置                 | 取消后可直接接管该实体的渲染                                                                                                                                         |
| `RenderLivingEvent`                             | 渲染活体事件                        |
| `RenderNameTagEvent`                            | 渲染名字标签事件                    |
| `RenderPlayerEvent$Post`                        | 渲染玩家事件－后置                 |
| `RenderPlayerEvent$Pre`                         | 渲染玩家事件－前置                 |
| `RenderPlayerEvent`                             | 渲染玩家事件                        |
| `RenderTooltipEvent$Color`                      | 渲染提示框事件－颜色               |
| `RenderTooltipEvent$GatherComponents`           | 渲染提示框事件－收集组件           |
| `RenderTooltipEvent$Pre`                        | 渲染提示框事件－前置               |
| `RenderTooltipEvent`                            | 渲染提示框事件                      |
| `ScreenEvent$BackgroundRendered`                | 界面事件－背景渲染                 |
| `ScreenEvent$CharacterTyped$Post`               | 界面事件－字符类型－后置          |
| `ScreenEvent$CharacterTyped$Pre`                | 界面事件－字符类型－前置          | 在界面处理字符输入之前触发                                                                                                                                           |
| `ScreenEvent$CharacterTyped`                    | 界面事件－字符类型                 |
| `ScreenEvent$Closing`                           | 界面事件－关闭                     |
| `ScreenEvent$Init$Post`                         | 界面事件－加载－后置              |
| `ScreenEvent$Init$Pre`                          | 界面事件－加载－前置              |
| `ScreenEvent$Init`                              | 界面事件－加载                     |
| `ScreenEvent$KeyInput`                          | 界面事件－按键输入                 |
| `ScreenEvent$KeyPressed$Post`                   | 界面事件－按下按键－后置          |
| `ScreenEvent$KeyPressed$Pre`                    | 界面事件－按下按键－前置          |
| `ScreenEvent$KeyPressed`                        | 界面事件－按下按键                 |
| `ScreenEvent$KeyReleased$Post`                  | 界面事件－松开按键－后置          |
| `ScreenEvent$KeyReleased$Pre`                   | 界面事件－松开按键－前置          |
| `ScreenEvent$KeyReleased`                       | 界面事件－松开按键                 |
| `ScreenEvent$MouseButtonPressed$Post`           | 界面事件－按下鼠标按键－后置      |
| `ScreenEvent$MouseButtonPressed$Pre`            | 界面事件－按下鼠标按键－前置      |
| `ScreenEvent$MouseButtonPressed`                | 界面事件－按下鼠标按键             |
| `ScreenEvent$MouseButtonReleased$Post`          | 界面事件－松开鼠标按键－后置      |
| `ScreenEvent$MouseButtonReleased$Pre`           | 界面事件－松开鼠标按键－前置      |
| `ScreenEvent$MouseButtonReleased`               | 界面事件－松开鼠标按键             |
| `ScreenEvent$MouseDragged$Post`                 | 界面事件－鼠标拖动－后置          |
| `ScreenEvent$MouseDragged$Pre`                  | 界面事件－鼠标拖动－前置          |
| `ScreenEvent$MouseDragged`                      | 界面事件－鼠标拖动                 |
| `ScreenEvent$MouseInput`                        | 界面事件－鼠标输入                 |
| `ScreenEvent$MouseScrolled$Post`                | 界面事件－鼠标滚轮－后置          |
| `ScreenEvent$MouseScrolled$Pre`                 | 界面事件－鼠标滚轮－前置          |
| `ScreenEvent$MouseScrolled`                     | 界面事件－鼠标滚轮                 |
| `ScreenEvent$Opening`                           | 界面事件－打开                     |
| `ScreenEvent$Render$Post`                       | 界面事件－渲染－后置              |
| `ScreenEvent$Render$Pre`                        | 界面事件－渲染－前置              |
| `ScreenEvent$Render`                            | 界面事件－渲染                     |
| `ScreenEvent$RenderInventoryMobEffects`         | 界面事件－渲染背包状态效果         | 可用于选择效果显示的大小（完整或紧凑），甚至完全隐藏或替换原版渲染                                                                                                   |
| `ScreenEvent`                                   | 界面事件                            |
| `ScreenshotEvent`                               | 截图事件                            |
| `TextureAtlasStitchedEvent`                     | 纹理图集缝合事件                    |
| `ToastAddEvent`                                 | `Toast` 添加事件                    | `Toast`: 玩家解锁新的制作配方或加载新世界时右上角显示的文本框                                                                                                        |
| `ViewportEvent$ComputeCameraAngles`             | 视口事件－计算相机角度             |
| `ViewportEvent$ComputeFogColor`                 | 视口事件－计算雾颜色               |
| `ViewportEvent$ComputeFov`                      | 视口事件－计算 FOV               |
| `ViewportEvent$RenderFog`                       | 视口事件－渲染雾                   |
| `ViewportEvent`                                 | 视口事件                            |
| `RegisterTicketControllersEvent`                | 注册 `Ticket` 控制器事件            |
| `GatherDataEvent`                               | 收集数据事件                        | 数据生成器是一种以编程方式生成模组 `assets` 和 `data` 的方法。它允许在代码中定义这些文件的内容并自动生成它们，而无需担心具体细节                                     |
| `PlayerBrewedPotionEvent`                       | 玩家酿造药水事件                    |
| `PotionBrewEvent$Post`                          | 药水酿造事件                        | 后置                                                                                                                                                                 |
| `PotionBrewEvent$Pre`                           | 药水酿造事件                        | 前置                                                                                                                                                                 |
| `PotionBrewEvent`                               | 药水酿造事件                        |
| `RegisterBrewingRecipesEvent`                   | 注册酿造配方事件                    |
| `EnchantmentLevelSetEvent`                      | 附魔等级设定事件                    |
| `GetEnchantmentLevelEvent`                      | 获取附魔等级事件                    |
| `ItemEvent`                                     | 物品事件                            |
| `ItemExpireEvent`                               | 物品过期事件                        | 物品掉落在地上一段时间后会过期                                                                                                                                       |
| `ItemTossEvent`                                 | 物品投掷事件                        |
| `AnimalTameEvent`                               | 动物驯服事件                        |
| `BabyEntitySpawnEvent`                          | 婴儿实体生成事件                    | 比如两个动物繁殖出一个小的                                                                                                                                           |
| `EffectParticleModificationEvent`               | 影响粒子修改事件                    |
| `EnderManAngerEvent`                            | 末影人愤怒事件                      |
| `FinalizeSpawnEvent`                            | 完成生成事件                        |
| `LivingAttackEvent`                             | 活体受攻击事件                      |
| `LivingBreatheEvent`                            | 活体呼吸事件                        |
| `LivingChangeTargetEvent`                       | 活体更改目标事件                    |
| `LivingConversionEvent$Post`                    | 活体转换事件－后置                 |
| `LivingConversionEvent$Pre`                     | 活体转换事件－前置                 |
| `LivingConversionEvent`                         | 活体转换事件                        | 例如苦力怕被雷击中变成闪电苦力怕                                                                                                                                     |
| `LivingDamageEvent`                             | 活体攻击事件                        |
| `LivingDeathEvent`                              | 活体死亡事件                        |
| `LivingDestroyBlockEvent`                       | 活体破坏方块事件                    |
| `LivingDropsEvent`                              | 活体掉落事件                        |
| `LivingDrownEvent`                              | 活体溺水事件                        |
| `LivingEntityUseItemEvent$Finish`               | 活体使用物品事件－完成             |
| `LivingEntityUseItemEvent$Start`                | 活体使用物品事件－开始             |
| `LivingEntityUseItemEvent$Stop`                 | 活体使用物品事件－停止             |
| `LivingEntityUseItemEvent$Tick`                 | 活体使用物品事件－`Tick`           |
| `LivingEntityUseItemEvent`                      | 活体使用物品事件                    |
| `LivingEquipmentChangeEvent`                    | 活体装备更换事件                    |
| `LivingEvent$LivingJumpEvent`                   | 活体事件－活体跳跃事件             |
| `LivingEvent$LivingVisibilityEvent`             | 活体事件－活体可见性事件           |
| `LivingEvent`                                   | 活体事件                            |
| `LivingExperienceDropEvent`                     | 活体经验掉落事件                    |
| `LivingFallEvent`                               | 活体下落事件                        |
| `LivingGetProjectileEvent`                      | 活体获取投掷物事件                  | 当活体尝试使用 `LivingEntity.getProjectile(ItemStack)` 方法获取投掷物时，会触发此事件                                                                                |
| `LivingHealEvent`                               | 活体治疗事件                        |
| `LivingHurtEvent`                               | 活体受伤事件                        |
| `LivingKnockBackEvent`                          | 活体击退事件                        |
| `LivingSwapItemsEvent$Hands`                    | 活体交换物品事件－手               |
| `LivingSwapItemsEvent`                          | 活体交换物品事件                    |
| `LivingUseTotemEvent`                           | 活体使用图腾事件                    |
| `MobDespawnEvent`                               | 怪物消失事件                        |
| `MobEffectEvent$Added`                          | 怪物效果事件－添加                 |
| `MobEffectEvent$Applicable`                     | 怪物效果事件－适用                 |
| `MobEffectEvent$Expired`                        | 怪物效果事件－到期                 |
| `MobEffectEvent$Remove`                         | 怪物效果事件－移除                 |
| `MobEffectEvent`                                | 怪物效果事件                        |
| `MobSpawnEvent$PositionCheck`                   | 怪物生成事件－坐标检查             |
| `MobSpawnEvent$SpawnPlacementCheck`             | 怪物移动事件－生成位置检查         |
| `MobSpawnEvent`                                 | 怪物生成事件                        |
| `MobSplitEvent`                                 | 怪物分裂事件                        |
| `ShieldBlockEvent`                              | 盾牌格挡事件                        |
| `SpawnClusterSizeEvent`                         | 生成簇大小事件                      |
| `AdvancementEvent$AdvancementEarnEvent`         | 进度事件－进度达成事件             |
| `AdvancementEvent$AdvancementProgressEvent`     | 进度事件－进度进展事件             |
| `AdvancementEvent`                              | 进度事件                            |
| `AnvilRepairEvent`                              | 铁砧修复事件                        |
| `ArrowLooseEvent`                               | 箭发射事件                          | 当玩家停止使用弓时会被触发，可获得发射之前的蓄力进度                                                                                                                 |
| `ArrowNockEvent`                                | 箭上膛事件                          | 当玩家开始使用弓时会被触发                                                                                                                                           |
| `AttackEntityEvent`                             | 攻击实体事件                        |
| `BonemealEvent`                                 | 骨粉事件                            |
| `CanContinueSleepingEvent`                      | 可以继续睡觉事件                    |
| `CanPlayerSleepEvent`                           | 玩家可以睡觉事件                    |
| `CriticalHitEvent`                              | 致命一击事件                        | 当玩家对实体造成致命一击时触发                                                                                                                                       |
| `ItemEntityPickupEvent$Post`                    | 物品实体拾取事件－后置             |
| `ItemEntityPickupEvent$Pre`                     | 物品实体拾取事件－前置             |
| `ItemEntityPickupEvent`                         | 物品实体拾取事件                    |
| `ItemFishedEvent`                               | 物品被钓上来事件                    |
| `ItemTooltipEvent`                              | 物品提示框事件                      |
| `PermissionsChangedEvent`                       | 权限更改事件                        |
| `PlayerContainerEvent$Close`                    | 玩家 容器事件－关闭        |
| `PlayerContainerEvent$Open`                     | 玩家 容器事件－打开        |
| `PlayerContainerEvent`                          | 玩家 容器事件               |
| `PlayerDestroyItemEvent`                        | 玩家销毁物品事件                    |
| `PlayerEvent$BreakSpeed`                        | 玩家事件－破坏速度                 | 当玩家尝试破坏方块时触发                                                                                                                                             |
| `PlayerEvent$Clone`                             | 玩家事件－克隆                     | 通常来讲，要么是死亡造成的，要么是从跨世界传送造成的                                                                                                                 |
| `PlayerEvent$HarvestCheck`                      | 玩家事件－收获检查                 | 当玩家尝试收获作物时触发                                                                                                                                             |
| `PlayerEvent$ItemCraftedEvent`                  | 玩家事件－物品合成事件             |
| `PlayerEvent$ItemSmeltedEvent`                  | 玩家事件－物品熔炼事件             |
| `PlayerEvent$LoadFromFile`                      | 玩家事件－从文件中加载             |
| `PlayerEvent$NameFormat`                        | 玩家事件－名称格式化               | 检索玩家名时触发                                                                                                                                                     |
| `PlayerEvent$PlayerChangeGameModeEvent`         | 玩家事件－玩家改变游戏模式事件     |
| `PlayerEvent$PlayerChangedDimensionEvent`       | 玩家事件－玩家改变维度事件         |
| `PlayerEvent$PlayerLoggedInEvent`               | 玩家事件－玩家登录事件             |
| `PlayerEvent$PlayerLoggedOutEvent`              | 玩家事件－玩家登出事件             |
| `PlayerEvent$PlayerRespawnEvent`                | 玩家事件－玩家重生事件             |
| `PlayerEvent$SaveToFile`                        | 玩家事件－保存到文件               |
| `PlayerEvent$StartTracking`                     | 玩家事件－开始跟踪                 | 玩家开始接收实体的状态更新，例如运动                                                                                                                                 |
| `PlayerEvent$StopTracking`                      | 玩家事件－结束跟踪                 |
| `PlayerEvent$TabListNameFormat`                 | 玩家事件－玩家列表名字格式化       |
| `PlayerEvent`                                   | 玩家事件                            |
| `PlayerFlyableFallEvent`                        | 玩家可飞行时坠落事件                |
| `PlayerHeartTypeEvent`                          | 玩家 心 类型事件                    |
| `PlayerInteractEvent$EntityInteract`            | 玩家交互事件－实体交互             |
| `PlayerInteractEvent$EntityInteractSpecific`    | 玩家交互事件－具体的实体交互       | 当玩家右键实体，双方都会触发                                                                                                                                         |
| `PlayerInteractEvent$LeftClickBlock`            | 玩家交互事件－左键方块             |
| `PlayerInteractEvent$LeftClickEmpty`            | 玩家交互事件－对空左键             |
| `PlayerInteractEvent$RightClickBlock`           | 玩家交互事件－右键方块             |
| `PlayerInteractEvent$RightClickEmpty`           | 玩家交互事件－对空右键             |
| `PlayerInteractEvent$RightClickItem`            | 玩家交互事件－右键物品             |
| `PlayerInteractEvent`                           | 玩家交互事件                        |
| `PlayerNegotiationEvent`                        | 玩家协商事件                        | 当连接开始 `Forge` 握手时，服务器上会触发此事件，`Forge` 将等待所有排队的工作完成，然后再继续进行登录过程                                                            |
| `PlayerRespawnPositionEvent`                    | 玩家重生位置事件                    |
| `PlayerSetSpawnEvent`                           | 玩家设置重生点事件                  |
| `PlayerSpawnPhantomsEvent`                      | 玩家生成幻影事件                    |
| `PlayerWakeUpEvent`                             | 玩家唤醒事件                        |
| `PlayerXpEvent$LevelChange`                     | 玩家经验事件－等级变化             |
| `PlayerXpEvent$PickupXp`                        | 玩家经验事件－拾取经验             |
| `PlayerXpEvent$XpChange`                        | 玩家经验事件－经验变化             |
| `PlayerXpEvent`                                 | 玩家经验事件                        |
| `TradeWithVillagerEvent`                        | 与村民贸易事件                      |
| `UseItemOnBlockEvent`                           | 对方块使用物品事件                  |
| `EntityAttributeCreationEvent`                  | 实体属性创建事件                    |
| `EntityAttributeModificationEvent`              | 实体属性修改事件                    |
| `EntityEvent$EnteringSection`                   | 实体事件－进入生物群系             |
| `EntityEvent$EntityConstructing`                | 实体事件－实体构造                 |
| `EntityEvent$Size`                              | 实体事件－大小                     |
| `EntityEvent`                                   | 实体事件                            |
| `EntityJoinLevelEvent`                          | 实体加入世界事件                    |
| `EntityLeaveLevelEvent`                         | 实体离开世界事件                    |
| `EntityMobGriefingEvent`                        | 实体怪物破坏事件                    |
| `EntityMountEvent`                              | 实体挂载事件                        |
| `EntityStruckByLightningEvent`                  | 实体被闪电击中事件                  |
| `EntityTeleportEvent$ChorusFruit`               | 实体传送事件－紫颂果               |
| `EntityTeleportEvent$EnderEntity`               | 实体传送事件－末影实体             | 在末影人或潜影贝随机传送之前触发                                                                                                                                                         |
| `EntityTeleportEvent$EnderPearl`                | 实体传送事件－末影珍珠             |
| `EntityTeleportEvent$SpreadPlayersCommand`      | 实体传送事件－随机传送命令         | `/spreadplayers` 命令                                                                                                                                                |
| `EntityTeleportEvent$TeleportCommand`           | 实体传送事件－传送命令             |
| `EntityTeleportEvent`                           | 实体传送事件                        |
| `EntityTravelToDimensionEvent`                  | 实体前往维度事件                    |
| `ProjectileImpactEvent`                         | 投掷物撞击事件                      |
| `SpawnPlacementRegisterEvent`                   | 生成放置注册表事件                  | 此事件允许每个 `EntityType` 注册或修改 `SpawnPlacements.SpawnPredicate`                                                                                                  |
| `FurnaceFuelBurnTimeEvent`                      | 融炉燃料燃烧时间事件                |
| `CreateFluidSourceEvent`                        | 创建流体源事件                      |
| `CropGrowEvent$Post`                            | 农作物生长事件－后置               |
| `CropGrowEvent$Pre`                             | 农作物生长事件－前置               |
| `CropGrowEvent`                                 | 农作物生长事件                      |
| `AlterGroundEvent`                              | 改变土地事件                        |
| `BlockDropsEvent`                               | 方块掉落事件                        |
| `BlockEvent$BlockToolModificationEvent`         | 方块事件－方块被工具改变事件       | 当工具与此块交互以更改其状态时触发。例如：用于确定斧头是否可以砍伐原木                                                                                               |
| `BlockEvent$BreakEvent`                         | 方块事件－破坏事件                 |
| `BlockEvent$EntityMultiPlaceEvent`              | 方块事件－实体多摆放事件           | 当单个方块放置触发多个块的创建时触发                                                                                                                                 |
| `BlockEvent$EntityPlaceEvent`                   | 方块事件－实体摆放事件             |
| `BlockEvent$FarmlandTrampleEvent`               | 方块事件－践踏农田事件             |
| `BlockEvent$FluidPlaceBlockEvent`               | 方块事件－流体放置方块事件         |
| `BlockEvent$NeighborNotifyEvent`                | 方块事件－邻居更新事件             | 当块上发生物理更新时触发。此事件充当 `Mod` 检测物理更新的一种方式，与 `BUD` 开关的作用相同。该事件仅在服务器上调用                                                   |
| `BlockEvent$PortalSpawnEvent`                   | 方块事件－传送门生成事件           |
| `BlockEvent`                                    | 方块事件                            |
| `BlockGrowFeatureEvent`                         | 方块生长特性事件－例如树苗长成树   |
| `ChunkDataEvent$Load`                           | 区块数据事件－加载                 |
| `ChunkDataEvent$Save`                           | 区块数据事件－保存                 |
| `ChunkDataEvent`                                | 区块数据事件                        |
| `ChunkEvent$Load`                               | 区块事件－加载                     |
| `ChunkEvent$Unload`                             | 区块事件－卸载                     |
| `ChunkEvent`                                    | 区块事件                            |
| `ChunkTicketLevelUpdatedEvent`                  | 区块 `Ticket Level` 加载事件        |
| `ChunkWatchEvent$Sent`                          | 区块观测事件－已发送               |
| `ChunkWatchEvent$UnWatch`                       | 区块观测事件－解除观测             |
| `ChunkWatchEvent$Watch`                         | 区块观测事件－观测                 |
| `ChunkWatchEvent`                               | 区块观测事件                        | 在服务端向客户端发送区块包的时候回调                                                                                                                                 |
| `ExplosionEvent$Detonate`                       | 爆炸事件－引爆                     |
| `ExplosionEvent$Start`                          | 爆炸事件－开始                     |
| `ExplosionEvent`                                | 爆炸事件                            |
| `ExplosionKnockbackEvent`                       | 爆炸击退事件                        |
| `LevelEvent$CreateSpawnPosition`                | 世界事件－创建生成位置             |
| `LevelEvent$Load`                               | 世界事件－加载                     |
| `LevelEvent$PotentialSpawns`                    | 世界事件－潜在生成                 | 当构建可以在指定位置生成的所有可能实体的列表时触发                                                                                                                   |
| `LevelEvent$Save`                               | 世界事件－保存                     |
| `LevelEvent$Unload`                             | 世界事件－卸载                     |
| `LevelEvent`                                    | 世界事件                            |
| `NoteBlockEvent$Change`                         | 音符盒事件－更改                   |
| `NoteBlockEvent$Play`                           | 音符盒事件－播放                   |
| `NoteBlockEvent`                                | 音符盒事件                          |
| `PistonEvent$Post`                              | 活塞事件－后置                     |
| `PistonEvent$Pre`                               | 活塞事件－前置                     |
| `PistonEvent`                                   | 活塞事件                            |
| `SleepFinishedTimeEvent`                        | 睡觉结束时间事件                    |
| `ServerAboutToStartEvent`                       | 服务器即将启动事件                  |
| `ServerLifecycleEvent`                          | 服务器生命周期事件                  |
| `ServerStartedEvent`                            | 服务器已启动事件                    |
| `ServerStartingEvent`                           | 服务器启动中事件                    |
| `ServerStoppedEvent`                            | 服务器已关闭事件                    |
| `ServerStoppingEvent`                           | 服务器关闭中事件                    |
| `EntityTickEvent$Post`                          | 实体游戏刻事件－后置             |
| `EntityTickEvent$Pre`                           | 实体游戏刻事件－前置             |
| `EntityTickEvent`                               | 实体游戏刻事件                    |
| `LevelTickEvent$Post`                           | 世界游戏刻事件－后置             |
| `LevelTickEvent$Pre`                            | 世界游戏刻事件－前置             |
| `LevelTickEvent`                                | 世界游戏刻事件                    |
| `PlayerTickEvent$Post`                          | 玩家游戏刻事件－后置             |
| `PlayerTickEvent$Pre`                           | 玩家游戏刻事件－前置             |
| `PlayerTickEvent`                               | 玩家游戏刻事件                    |
| `ServerTickEvent$Post`                          | 服务器游戏刻事件－后置           |
| `ServerTickEvent$Pre`                           | 服务器游戏刻事件－前置           |
| `ServerTickEvent`                               | 服务器游戏刻事件                  |
| `VillageSiegeEvent`                             | 村庄袭击事件                        |
| `VillagerTradesEvent`                           | 村民交易事件                        |
| `WandererTradesEvent`                           | 流浪商人交易事件                    |
| `AddPackFindersEvent`                           | 添加数据包查找器事件                |
| `AddReloadListenerEvent`                        | 添加重载监听器事件                  |
| `AnvilUpdateEvent`                              | 铁砧更新事件                        |
| `BuildCreativeModeTabContentsEvent`             | 构建创造模式选项卡内容事件          |
| `CommandEvent`                                  | 命令事件                            |
| `DifficultyChangeEvent`                         | 难度更改事件                        |
| `GameShuttingDownEvent`                         | 游戏关闭中事件                      |
| `GrindstoneEvent$OnPlaceItem`                   | 砂轮事件－物品置于其上             |
| `GrindstoneEvent$OnTakeItem`                    | 砂轮事件－作用物品                 |
| `GrindstoneEvent`                               | 砂轮事件                            |
| `ItemAttributeModifierEvent`                    | 物品属性修改事件                    |
| `ItemStackedOnOtherEvent`                       | 物品堆叠在其它物品上事件            | 物品栏中当你试图将一堆物品堆叠到另一堆物品上                                                                                                                         |
| `LootTableLoadEvent`                            | 战利品表加载事件                    |
| `ModMismatchEvent`                              | 模组不匹配事件                      |
| `ModifyDefaultComponentsEvent`                  | 修改默认组件事件                    |
| `OnDatapackSyncEvent`                           | 数据包同步事件                      |
| `PlayLevelSoundEvent$AtEntity`                  | 播放世界声音事件－在实体上         |
| `PlayLevelSoundEvent$AtPosition`                | 播放世界声音事件－在坐标上         |
| `PlayLevelSoundEvent`                           | 播放世界声音事件                    |
| `RegisterCommandsEvent`                         | 注册命令事件                        |
| `RegisterGameTestsEvent`                        | 注册游戏测试事件                    |
| `RegisterStructureConversionsEvent`             | 注册结构转换事件                    | 在旧版本存档转换到当前版本时注册一个结构转换器                                                                                                                       |
| `ServerChatEvent`                               | 服务器聊天事件                      |
| `StatAwardEvent`                                | 统计 Award 事件                   |
| `TagsUpdatedEvent`                              | 标签更新事件                        | `i18n` 标签之类的                                                                                                                                                    |
| `VanillaGameEvent`                              | 原版游戏事件                        |
| `RegisterCauldronFluidContentEvent`             | 注册炼药锅液体内容事件              |
| `RegisterConfigurationTasksEvent`               | 注册配置任务事件                    | 配置任务在玩家进入服务器时在客户端方面发送一些元数据，服务器接受它们                                                                                                 |
| `RegisterPayloadHandlersEvent`                  | 注册有效负载处理程序事件            | `Networking` 的一些未稳定细节                                                                                                                                        |
| `DataMapsUpdatedEvent`                          | 数据 `Maps` 更新事件                |
| `RegisterDataMapTypesEvent`                     | 注册数据 `Map` 类型事件             |
| `DataPackRegistryEvent$NewRegistry`             | 数据包注册事件－新注册表           |
| `DataPackRegistryEvent`                         | 数据包注册表事件                    |
| `IdMappingEvent`                                | `ID` 映射事件                       |
| `ModifyRegistriesEvent`                         | 修改注册表事件                      |
| `NewRegistryEvent`                              | 新注册表事件                        |
| `RegisterEvent`                                 | 注册事件                            |
| `PermissionGatherEvent$Handler`                 | 权限收集事件－处理程序             |
| `PermissionGatherEvent$Nodes`                   | 权限收集事件－节点                 |
| `PermissionGatherEvent`                         | 权限收集事件                        |
