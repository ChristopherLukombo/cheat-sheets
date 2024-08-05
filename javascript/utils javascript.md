```javascript

 static passwordMatch(control: AbstractControl): ValidationErrors | null {
    const password = control.get('password')!.value;
    const confirmPassword = control.get('confirmPassword')!.value;
    return password !== confirmPassword ? { matchingError: true } : null;
  }
```