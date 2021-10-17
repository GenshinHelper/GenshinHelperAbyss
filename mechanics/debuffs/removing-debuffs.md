# Removing Debuffs

## Mechanics

Removing a debuff (**cleansing**) can only be done by applying an element to a character and triggering an **Elemental Reaction** with the debuff element. 

### Strong/Weak Cleanses

Abilities that apply elements that are **strong** against the debuff element work the best. Using an element that is **weak** against the debuff may only **partially cleanse** the element, and require multiple applications/reactions before fulling removing the debuff.

|                    Debuff                    |                    Strong                   |                                         Neutral                                         |                     Weak                     |                                     Not Effective                                     |
| :------------------------------------------: | :-----------------------------------------: | :-------------------------------------------------------------------------------------: | :------------------------------------------: | :-----------------------------------------------------------------------------------: |
|  ![](../../.gitbook/assets/pyro_small.png)   | ![](../../.gitbook/assets/hydro_small.png)  |  ![](../../.gitbook/assets/electro_small.png)![](../../.gitbook/assets/anemo_small.png) |   ![](../../.gitbook/assets/cryo_small.png)  |                                           -                                           |
|  ![](../../.gitbook/assets/hydro_small.png)  |                      -                      |                        ![](../../.gitbook/assets/anemo_small.png)                       |   ![](../../.gitbook/assets/pyro_small.png)  | ![](../../.gitbook/assets/cryo_small.png)![](../../.gitbook/assets/electro_small.png) |
|   ![](../../.gitbook/assets/cryo_small.png)  |  ![](../../.gitbook/assets/pyro_small.png)  |   ![](../../.gitbook/assets/hydro_small.png)![](../../.gitbook/assets/anemo_small.png)  | ![](../../.gitbook/assets/electro_small.png) |                                           -                                           |
| ![](../../.gitbook/assets/electro_small.png) |  ![](../../.gitbook/assets/cryo_small.png)  |   ![](../../.gitbook/assets/pyro_small.png)![](../../.gitbook/assets/anemo_small.png)   |                       -                      |                       ![](../../.gitbook/assets/hydro_small.png)                      |

The weaker the cleanse, the more applications of the element it will take to remove the debuff. Table below shows the number of reactions that need to be triggered.

| Type         | Strong | Neutral | Weak |
| ------------ | :----: | :-----: | :--: |
| Stage Debuff |    1   |    2    |   4  |
| Aura Debuff  |    1   |    1    |   2  |

### **Stage Debuff**

Stage debuffs apply a fixed amount of element to your characters, which slowly decreases over time. If this debuff is **partially cleansed**, it will reduce the duration of the debuff.

In the example below, Xinyan's shield **partially cleanses** the ![](../../.gitbook/assets/electro_small.png) debuff, cutting the duration in half. Notice how Ganyu is still affected by ![](../../.gitbook/assets/electro_small.png)after it runs out on Xinyan.

![](../../.gitbook/assets/cleanse_partial.gif)

In order to clear stage debuffs from your entire team, activate the talent which applies the element, then cycle through your team until the debuffs are cleared. You may need to do this multiple times if you are using a **weak cleanse**.

![](../../.gitbook/assets/cleans_team.gif)

{% hint style="info" %}
Stage debuffs apply a variable amount of **Elemental Gauge**, but for the upper floors of abyss this will usually be **2 Units**.
{% endhint %}

### Aura Debuff

Aura debuffs apply a fixed amount of element to your active character. However, **switching characters will refresh the element**. Make sure to fully cleanse the debuff before switching off if using a **weak cleanse**.

{% hint style="danger" %}
 Using a **weak cleanse** from a Shield will not work since it relies on switching characters!
{% endhint %}

![](../../.gitbook/assets/cleanse_noeffect.gif)

The example above shows attempting to cleanse![](../../.gitbook/assets/hydro_small.png)with ![](../../.gitbook/assets/pyro_small.png)(**weak cleanse**) from a shield. In order to clear the debuff, we need **2 applications** of ![](../../.gitbook/assets/pyro_small.png). However, in order to do this we have to switch characters, which causes the debuff to refresh. The end result is that Xinyan's skill cannot cleanse the  ![](../../.gitbook/assets/hydro_small.png) debuff!

{% hint style="info" %}
Aura debuffs apply **1 Unit **of **Elemental Gauge**.
{% endhint %}

### Reaction Trigger

The order that the elements are applied matters. You want to make sure that the **debuff** element is applied **first**, followed by the element from the **cleanse second**. The source that **triggers the reaction** determines if the reaction affects you or the enemy.

In the example below, the ![](../../.gitbook/assets/electro_small.png)debuff is applied, and cleansed by ![](../../.gitbook/assets/pyro_small.png)from Bennet. This triggers **Overload**, but Bennet doesn't take damage, and instead the Slimes take damage.

![Electro Debuff followed by Bennet Pyro](../../.gitbook/assets/cleanse_overload_nodmg.gif)

In the next example, ![](../../.gitbook/assets/pyro_small.png)is applied from Bennet, followed by ![](../../.gitbook/assets/electro_small.png)from the debuff. This triggers **Overload**, but Bennet takes damage.

![Bennet Pyro followed by Electro Debuff](../../.gitbook/assets/cleanse_overload_dmg.gif)

## Team Cleansers

These characters are able to apply elements to other members of the party, making them ideal for cleansing.

### Continuous Application

These talents will periodically apply elements to the active character **every few seconds**.

For weaker cleanses, you may need to wait for multiple ticks before the element is removed.

|                       Character                       |               Applied Element               | Talent | Timer |
| :---------------------------------------------------: | :-----------------------------------------: | :----: | :---: |
| ![](../../.gitbook/assets/ui_avataricon_bennett.png)  |  ![](../../.gitbook/assets/pyro_small.png)  |  Burst |   1s  |
| ![](../../.gitbook/assets/ui_avataricon_barbara.png)  | ![](../../.gitbook/assets/hydro_small.png)  |  Skill |   5s  |
|   ![](../../.gitbook/assets/ui_avataricon_jean.png)   | ![](../../.gitbook/assets/anemo_small.png)  |  Burst |   1s  |

### Shields

Shields apply their element **when used**, but again whenever you **switch characters**.

For weaker cleanses, you may need to switch multiple times before the element is removed.

|                       Character                      |               Applied Element              | Talent |
| :--------------------------------------------------: | :----------------------------------------: | :----: |
|  ![](../../.gitbook/assets/ui_avataricon_diona.png)  | ![](../../.gitbook/assets/cryo_small.png)  |  Skill |
| ![](../../.gitbook/assets/ui_avataricon_xinyan.png)  | ![](../../.gitbook/assets/pyro_small.png)  |  Skill |

## Self Cleansers

These talents will only apply the element to themselves. They are not useful for clearing **stage debuffs** from your team, but can be effective at clearing **aura debuffs.**

|                       Character                       |                Applied Element                | Talent | Timer |
| :---------------------------------------------------: | :-------------------------------------------: | :----: | :---: |
|  ![](../../.gitbook/assets/ui_avataricon_beidou.png)  |  ![](../../.gitbook/assets/electro_small.png) |  Skill |   -   |
|  ![](../../.gitbook/assets/ui_avataricon_razor.png)   | ![](../../.gitbook/assets/electro_small.png)  |  Burst |   2s  |
| ![](../../.gitbook/assets/ui_avataricon_xingqiu.png)  |  ![](../../.gitbook/assets/hydro_small.png)   |  Skill |   -   |
