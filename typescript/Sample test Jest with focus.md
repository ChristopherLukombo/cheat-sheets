```typescript


  describe('ngAfterViewInit', () => {
    it('shoult set focus to username input after the view has been initialized', () => {
      // GIVEN
      const node = {
        focus: jest.fn(),
      };
      comp.username = new ElementRef(node);

      // WHEN
      comp.ngAfterViewInit();

      // THEN
      expect(node.focus).toHaveBeenCalled();
    });
  });
```