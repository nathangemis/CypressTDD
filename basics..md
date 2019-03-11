# Learn Cypress Basics

### Write your first test

create in integration folder a new file *sample.spec.js* and open it.

### Describe your group test 
```
describe('Name of your group test',function(){
  

})
```
### Create your first test suite
```
describe('My First Test', function(){
  it('Name of your test suite',function()=>{
    
  })

})
```

### Connect to a server or website 
```
describe('Name of your group test',function(){
  it('Visits the kitchen Sink',function()=>{
    cy.visit('https://example.cypress.io')
  })

})
```

### First test suite
```
describe('My First Test', function(){
    it('Visits the kitchen Sink', function(){
        
        cy.visit('https://example.cypress.io')

        cy.contains('type').click()
        cy.url().should('include','/commands/actions')

        cy.get('.action-email')
        .type('fake@email.com')
        .should('have.value','fake@email.com')
    })
})
```
