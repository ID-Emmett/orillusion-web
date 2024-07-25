# Class: Rigidbody

Rigidbody Component
Rigid bodies can endow game objects with physical properties, allowing them to be controlled by the physics system and subjected to forces and torques, thus achieving realistic motion effects.

## Hierarchy

- `ComponentBase`

  ↳ **`Rigidbody`**

### Constructors

- [constructor](Rigidbody.md#constructor)

### Properties

- [object3D](Rigidbody.md#object3d)
- [isDestroyed](Rigidbody.md#isdestroyed)

### Accessors

- [friction](Rigidbody.md#friction)
- [rollingFriction](Rigidbody.md#rollingfriction)
- [restitution](Rigidbody.md#restitution)
- [btRigidbodyInited](Rigidbody.md#btrigidbodyinited)
- [btRigidbody](Rigidbody.md#btrigidbody)
- [mass](Rigidbody.md#mass)
- [velocity](Rigidbody.md#velocity)
- [angularVelocity](Rigidbody.md#angularvelocity)
- [isKinematic](Rigidbody.md#iskinematic)
- [isTrigger](Rigidbody.md#istrigger)
- [eventDispatcher](Rigidbody.md#eventdispatcher)
- [isStart](Rigidbody.md#isstart)
- [transform](Rigidbody.md#transform)
- [enable](Rigidbody.md#enable)

### Methods

- [init](Rigidbody.md#init)
- [start](Rigidbody.md#start)
- [addInitedFunction](Rigidbody.md#addinitedfunction)
- [removeInitedFunction](Rigidbody.md#removeinitedfunction)
- [onUpdate](Rigidbody.md#onupdate)
- [destroy](Rigidbody.md#destroy)
- [stop](Rigidbody.md#stop)
- [onEnable](Rigidbody.md#onenable)
- [onDisable](Rigidbody.md#ondisable)
- [onLateUpdate](Rigidbody.md#onlateupdate)
- [onBeforeUpdate](Rigidbody.md#onbeforeupdate)
- [onCompute](Rigidbody.md#oncompute)
- [onGraphic](Rigidbody.md#ongraphic)
- [onParentChange](Rigidbody.md#onparentchange)
- [onAddChild](Rigidbody.md#onaddchild)
- [onRemoveChild](Rigidbody.md#onremovechild)
- [cloneTo](Rigidbody.md#cloneto)
- [copyComponent](Rigidbody.md#copycomponent)
- [beforeDestroy](Rigidbody.md#beforedestroy)

## Constructors

### constructor

• **new Rigidbody**(): [`Rigidbody`](Rigidbody.md)

#### Returns

[`Rigidbody`](Rigidbody.md)

#### Inherited from

ComponentBase.constructor

## Properties

### object3D

• **object3D**: `Object3D` = `null`

owner object3D

#### Inherited from

ComponentBase.object3D

#### Defined in

[src/components/ComponentBase.ts:17](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L17)

___

### isDestroyed

• `Optional` **isDestroyed**: `boolean`

#### Inherited from

ComponentBase.isDestroyed

#### Defined in

[src/components/ComponentBase.ts:38](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L38)

## Accessors

### friction

• `get` **friction**(): `number`

Get friction value

#### Returns

`number`

#### Defined in

[packages/physics/Rigidbody.ts:66](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L66)

• `set` **friction**(`value`): `void`

Set friction value

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

[packages/physics/Rigidbody.ts:72](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L72)

___

### rollingFriction

• `get` **rollingFriction**(): `number`

Get rolling friction value

#### Returns

`number`

#### Defined in

[packages/physics/Rigidbody.ts:79](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L79)

• `set` **rollingFriction**(`value`): `void`

Set rolling friction value

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

[packages/physics/Rigidbody.ts:85](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L85)

___

### restitution

• `get` **restitution**(): `number`

Get restitution value

#### Returns

`number`

#### Defined in

[packages/physics/Rigidbody.ts:92](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L92)

• `set` **restitution**(`value`): `void`

Set restitution value

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

[packages/physics/Rigidbody.ts:98](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L98)

___

### btRigidbodyInited

• `get` **btRigidbodyInited**(): `boolean`

Check if rigidbody inited

#### Returns

`boolean`

#### Defined in

[packages/physics/Rigidbody.ts:105](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L105)

___

### btRigidbody

• `get` **btRigidbody**(): [`btRigidBody`](Ammo.btRigidBody.md)

Return internal Ammo.btRigidBody

#### Returns

[`btRigidBody`](Ammo.btRigidBody.md)

#### Defined in

[packages/physics/Rigidbody.ts:187](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L187)

___

### mass

• `get` **mass**(): `number`

Get mass value。

#### Returns

`number`

#### Defined in

[packages/physics/Rigidbody.ts:217](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L217)

• `set` **mass**(`value`): `void`

Set mass value。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `number` |

#### Returns

`void`

#### Defined in

[packages/physics/Rigidbody.ts:223](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L223)

___

### velocity

• `get` **velocity**(): `Vector3`

Get velocity value of current object

#### Returns

`Vector3`

#### Defined in

[packages/physics/Rigidbody.ts:241](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L241)

• `set` **velocity**(`value`): `void`

Set velocity value of current object

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `Vector3` |

#### Returns

`void`

#### Defined in

[packages/physics/Rigidbody.ts:247](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L247)

___

### angularVelocity

• `get` **angularVelocity**(): `Vector3`

Get the angular velocity value of current object

#### Returns

`Vector3`

#### Defined in

[packages/physics/Rigidbody.ts:256](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L256)

• `set` **angularVelocity**(`value`): `void`

Set the angular velocity value of current object

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `Vector3` |

#### Returns

`void`

#### Defined in

[packages/physics/Rigidbody.ts:263](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L263)

___

### isKinematic

• `get` **isKinematic**(): `boolean`

Check if the rigidbody affect physics system

#### Returns

`boolean`

#### Defined in

[packages/physics/Rigidbody.ts:269](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L269)

• `set` **isKinematic**(`value`): `void`

Set if the rigidbody affect physics system

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

[packages/physics/Rigidbody.ts:275](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L275)

___

### isTrigger

• `get` **isTrigger**(): `boolean`

#### Returns

`boolean`

#### Defined in

[packages/physics/Rigidbody.ts:279](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L279)

• `set` **isTrigger**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Defined in

[packages/physics/Rigidbody.ts:283](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L283)

___

### eventDispatcher

• `get` **eventDispatcher**(): `CEventDispatcher`

#### Returns

`CEventDispatcher`

#### Inherited from

ComponentBase.eventDispatcher

#### Defined in

[src/components/ComponentBase.ts:23](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L23)

• `set` **eventDispatcher**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `CEventDispatcher` |

#### Returns

`void`

#### Inherited from

ComponentBase.eventDispatcher

#### Defined in

[src/components/ComponentBase.ts:28](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L28)

___

### isStart

• `get` **isStart**(): `boolean`

#### Returns

`boolean`

#### Inherited from

ComponentBase.isStart

#### Defined in

[src/components/ComponentBase.ts:40](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L40)

___

### transform

• `get` **transform**(): `Transform`

Return the Transform component attached to the Object3D.

#### Returns

`Transform`

#### Inherited from

ComponentBase.transform

#### Defined in

[src/components/ComponentBase.ts:47](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L47)

___

### enable

• `get` **enable**(): `boolean`

Enable/disable components. The enabled components can be updated, while the disabled components cannot be updated.

#### Returns

`boolean`

#### Inherited from

ComponentBase.enable

#### Defined in

[src/components/ComponentBase.ts:68](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L68)

• `set` **enable**(`value`): `void`

Enable/disable components. The enabled components can be updated, while the disabled components cannot be updated.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`void`

#### Inherited from

ComponentBase.enable

#### Defined in

[src/components/ComponentBase.ts:54](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L54)

## Methods

### init

▸ **init**(): `void`

#### Returns

`void`

#### Overrides

ComponentBase.init

#### Defined in

[packages/physics/Rigidbody.ts:51](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L51)

___

### start

▸ **start**(): `void`

#### Returns

`void`

#### Overrides

ComponentBase.start

#### Defined in

[packages/physics/Rigidbody.ts:55](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L55)

___

### addInitedFunction

▸ **addInitedFunction**(`fun`, `thisObj`): `void`

Add init callback

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fun` | `Function` | callback function |
| `thisObj` | `Object` | this |

#### Returns

`void`

#### Defined in

[packages/physics/Rigidbody.ts:148](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L148)

___

### removeInitedFunction

▸ **removeInitedFunction**(`fun`, `thisObj`): `void`

Remove init callback

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fun` | `Function` | callback function |
| `thisObj` | `Object` | this |

#### Returns

`void`

#### Defined in

[packages/physics/Rigidbody.ts:156](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L156)

___

### onUpdate

▸ **onUpdate**(): `void`

#### Returns

`void`

#### Overrides

ComponentBase.onUpdate

#### Defined in

[packages/physics/Rigidbody.ts:191](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L191)

___

### destroy

▸ **destroy**(`force?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `force?` | `boolean` |

#### Returns

`void`

#### Overrides

ComponentBase.destroy

#### Defined in

[packages/physics/Rigidbody.ts:208](https://github.com/Orillusion/orillusion/blob/main/packages/physics/Rigidbody.ts#L208)

___

### stop

▸ **stop**(): `void`

#### Returns

`void`

#### Inherited from

ComponentBase.stop

#### Defined in

[src/components/ComponentBase.ts:114](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L114)

___

### onEnable

▸ **onEnable**(`view?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view?` | `View3D` |

#### Returns

`any`

#### Inherited from

ComponentBase.onEnable

#### Defined in

[src/components/ComponentBase.ts:115](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L115)

___

### onDisable

▸ **onDisable**(`view?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view?` | `View3D` |

#### Returns

`any`

#### Inherited from

ComponentBase.onDisable

#### Defined in

[src/components/ComponentBase.ts:116](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L116)

___

### onLateUpdate

▸ **onLateUpdate**(`view?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view?` | `View3D` |

#### Returns

`any`

#### Inherited from

ComponentBase.onLateUpdate

#### Defined in

[src/components/ComponentBase.ts:118](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L118)

___

### onBeforeUpdate

▸ **onBeforeUpdate**(`view?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view?` | `View3D` |

#### Returns

`any`

#### Inherited from

ComponentBase.onBeforeUpdate

#### Defined in

[src/components/ComponentBase.ts:119](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L119)

___

### onCompute

▸ **onCompute**(`view?`, `command?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view?` | `View3D` |
| `command?` | `GPUCommandEncoder` |

#### Returns

`any`

#### Inherited from

ComponentBase.onCompute

#### Defined in

[src/components/ComponentBase.ts:120](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L120)

___

### onGraphic

▸ **onGraphic**(`view?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `view?` | `View3D` |

#### Returns

`any`

#### Inherited from

ComponentBase.onGraphic

#### Defined in

[src/components/ComponentBase.ts:121](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L121)

___

### onParentChange

▸ **onParentChange**(`lastParent?`, `currentParent?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `lastParent?` | `Object3D` |
| `currentParent?` | `Object3D` |

#### Returns

`any`

#### Inherited from

ComponentBase.onParentChange

#### Defined in

[src/components/ComponentBase.ts:122](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L122)

___

### onAddChild

▸ **onAddChild**(`child`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `child` | `Object3D` |

#### Returns

`any`

#### Inherited from

ComponentBase.onAddChild

#### Defined in

[src/components/ComponentBase.ts:123](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L123)

___

### onRemoveChild

▸ **onRemoveChild**(`child`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `child` | `Object3D` |

#### Returns

`any`

#### Inherited from

ComponentBase.onRemoveChild

#### Defined in

[src/components/ComponentBase.ts:124](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L124)

___

### cloneTo

▸ **cloneTo**(`obj`): `void`

clone component data to target object3D

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `Object3D` | target object3D |

#### Returns

`void`

#### Inherited from

ComponentBase.cloneTo

#### Defined in

[src/components/ComponentBase.ts:131](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L131)

___

### copyComponent

▸ **copyComponent**(`from`): `this`

#### Parameters

| Name | Type |
| :------ | :------ |
| `from` | `this` |

#### Returns

`this`

#### Inherited from

ComponentBase.copyComponent

#### Defined in

[src/components/ComponentBase.ts:133](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L133)

___

### beforeDestroy

▸ **beforeDestroy**(`force?`): `void`

before release this component, object refrences are not be set null now.

#### Parameters

| Name | Type |
| :------ | :------ |
| `force?` | `boolean` |

#### Returns

`void`

#### Inherited from

ComponentBase.beforeDestroy

#### Defined in

[src/components/ComponentBase.ts:200](https://github.com/Orillusion/orillusion/blob/main/src/components/ComponentBase.ts#L200)
