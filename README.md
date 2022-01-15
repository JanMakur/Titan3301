```ts
interface GitHubAboutMeInterface {
  username:string | null | undefined;
  name: string | null | undefined;
  likes: string[] | string | null | undefined;
  hobby: string[] | string | null | undefined;
  worksat: string[] | string | null | undefined;
  telegram: string[] | string | undefined;
}
class GitHubAboutMe {
  username:string | null | undefined;
  name: string | null | undefined;
  likes: string[] | string | null | undefined;
  hobby: string[] | string | null | undefined;
  worksat: string[] | string | null | undefined;
  telegram: string[] | string | undefined:
  
  constructor(data:GitHubAboutMeInterface) {
    this.username = data.username;
    this.name = data.name;
    this.likes = data.likes;
    this.hobby = data.hobby;
    this.worksat = data.worksat;
    this.telegram = data.telegram;
  }
}
let self = {};
self.readme = new GitHubAboutMe({
  username:'Titan3301',
  name:undefined,
  likes:['TypeScript','JavaScript','C#','Rust'],
  hobby:['Programming'],
  worksat:undefined,
  telegram:'@Titan1337'
})
