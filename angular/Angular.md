```typescript

this.route.paramMap

      .pipe(

        take(1),

        flatMap((params: ParamMap) =>

          this.ordersService.getOrdersDetails(params.get('orderNumber')!)

        )

      )

      .subscribe(this.retrieveData, this.handleError)

      .add(this.afterCompletion);
      
```

Command Line
`npm audit

npm i -g npm-check-updates

ncu -u

npm i

npm audit fix

npx browserslist

ng serve --hmr -o`