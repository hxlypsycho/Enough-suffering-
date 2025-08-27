# Enough-suffering-
Make Money or u go suffer.
function getMultiplier() {
  // Use a skewed distribution to favor lower numbers (1.2 to 5)
  // and have a low probability for numbers over 5
  const cutoff = Math.random();
  if (cutoff < 0.8) { // 80% chance to be between 1.2 and 5
    return Math.random() * (5 - 1.2) + 1.2;
  } else { // 20% chance to be between 5 and 30
    return Math.random() * (30 - 5) + 5;
