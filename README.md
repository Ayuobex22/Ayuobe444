# Ayuobe444
svg {
  width: 1.5rem;
}
// For <Icon className="custom-class" />
svg.custom-class {
  path {
    fill: blue;
  }
}
// For <Stack className="custom-class">
svg.custom-class {
  // First layer (behind)
  path:nth-child(1) {
    fill: blue;
  }
  // Second layer (infront)
  path:nth-child(2) {
    fill: red;
  }
}
<p><Icon path={mdiAccount} /> User Profile</p>
<p><Icon path={mdiAccount} title="User Profile" /></p>
<button aria-label="User Profile"><Icon path={mdiAccount} /></button>
