# rn-udesk

[![GitHub license](https://img.shields.io/badge/license-MIT-blue)](./LICENSE)
[![npm](https://img.shields.io/badge/npm-1.0.0-green)](https://www.npmjs.com/package/rn-udesk)

## Getting started

`$ npm install rn-udesk --save`

### Mostly automatic installation

`$ react-native link rn-udesk-udesk`

## Usage
```js
import ReactNativeUdesk from 'rn-udesk';

// 以下是ReactNativeUdesk可使用的方法

/**
 * 用户信息，用于传入这些用户信息，供客服查看
 */
export interface IUserInfo {
    nickname?: string;
    email?: string;
    phone?: string;
    description?: string;
    domain:string;
    appKey:string;
    appId:string;
    sdkToken:string;  //是客户的唯一标识，用来识别身份，可以传userId
}

/**
 * 开始聊天
 * @param {IUserInfo} userInfo 用户信息
 */
export function startChat(userInfo?: IUserInfo): Promise<boolean>
```
