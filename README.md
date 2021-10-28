```ts
interface GitHubAboutMeInterface {
  username:string | null | undefined;
  name: string | null | undefined;
  likes: Array<string> | string | null | undefined;
  hobby: Array<string> | string | null | undefined;
  worksat: string | null | undefined;
}
class GitHubAboutMe {
  username:string | null | undefined;
  name: string | null | undefined;
  likes: Array<string> | string | null | undefined;
  hobby: Array<string> | string | null | undefined;
  worksat:string | null | undefined;
  
  constructor(data:GitHubAboutMeInterface) {
    this.username = data.username;
    this.name = data.name;
    this.likes = data.likes;
    this.hobby = data.hobby;
    this.worksat = data.worksat;
  }
}
let self = {};
self.readme = new GitHubAboutMe({
  username:'Titan3301',
  name:undefined,
  likes:['typescript' , 'javascript' , 'csharp'],
  hobby:['Programming'],
  worksat:undefined
})
