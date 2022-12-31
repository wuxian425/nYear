<img src="./src/logo.svg" width="100%" height="auto"/>

# nYear

Live broadcast information and countdown of New Year's Eve. 

## Develop

You need [`Node.js`](https://nodejs.org/) and `npm`.

### Install

```
npm i
```

### Build

```
npm run build
```

### Serve

```
npm run dev
```

### Logo

```JSX
<div
  style={{
    height: '100%',
    width: '100%',
    backgroundImage: 'radial-gradient(circle at 15px 15px, #BB8888, lightgray 2%, transparent 0%), radial-gradient(circle at 45px 45px, #BB8888, lightgray 2%, transparent 0%)',
    backgroundSize: '60px 60px',
    backgroundColor: '#F9F9F9',
    borderRadius: '6px',
    fontSize: '16px',
    fontWeight: 400,
    display: 'flex',
    alignItems: 'center',
    flexDirection: 'column',
    justifyContent: 'center',
    position: 'relative',
  }}
>
  <div 
    style={{
      borderBottom: '2px solid #E8E8E8',
      color: '#BB8888',
      display: 'flex',
      fontSize: '54px',
      fontWeight: 500,
      lineHeight: 0.75,
      letterSpacing: '2px',
      marginBottom: '4px',
      padding: '2px 0px',
    }}
  >
    <b style={{color: '#884444',fontWeight: 700}}>n</b>
    ew
    <b style={{color: '#884444',fontWeight: 700}}>Year</b>.
  </div>

  <div style={{
    color: '#DDAAAA',
    fontSize: '16px',
    fontStyle: '',
    letterSpacing: '6px',
    marginBottom: '16px',
  }}
  >
    nYear.ga
  </div>

  <div 
    style={{
      letterSpacing: '0.5px',
      color: '#666666',
    }}>
  跨年直播資訊與倒計時整理。
  </div>

  <small style={{
    background: '#F9F9F9',
    color: '#CCCCCC',
    fontSize: '12px',
    position: 'absolute',
    bottom: '5vh',
  }}
  >
    2023 BobYang.
  </small>
</div>
```

###### (c) 2022 BobYang.