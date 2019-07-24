# @express.ts/router
 A simple router to make it easy to use with Typescript for building efficient and scalable server-side applications, heavily inspired by <a href="https://spring.io" target="blank">Spring MVC</a>.


```typescript
import { RequestMapping, GetMapping, RequestMethod } from "@express.ts/router";
import { Controller, Request, Response, RequestParam } from "@express.ts/stereotype";


@Controller("/api")
export default class ApiController {

  /**
   * GET /api
   * List of API examples.
   */
  @GetMapping("")
  index (@Request() req: any,
         @Response() res: any) {
    res.render("api/index", {
      title: "API Examples"
    });
  }

}

```
