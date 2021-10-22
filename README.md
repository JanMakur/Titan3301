```ts
interface GitHubReadMeInterface {
  username:string | null | undefined;
  name: Array<string> | string | null | undefined;
  likes: Array<string> | string | null | undefined;
  hobby:string | null | undefined;
  worksat:string | null | undefined;
}
class GitHubReadMe {
  username:string | null | undefined;
  name: string | null | undefined;
  likes: Array<string> | string | null | undefined;
  hobby: Array<string> | string | null | undefined;
  worksat:string | null | undefined;
  
  constructor(data:GitHubReadMeInterface) {
    this.username = data.username;
    this.name = data.name;
    this.likes = data.likes;
    this.hobby = data.hobby;
    this.worksat = data.worksat;
  }
}
let self = {};
self.readme = new GitHubReadMe({
  username:'Titan3301',
  name:undefined,
  likes:['typescript' , 'javascript' , 'rust'],
  hobby:['Programming'],
  worksat:undefined
})
