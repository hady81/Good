# لعبة شد الحبل (Tug of War) 🏆

let ropePosition = 0;
document.getElementById("pull-left").addEventListener("click", () => {
    ropePosition -= 10;
    updateRope();
});
document.getElementById("pull-right").addEventListener("click", () => {
    ropePosition += 10;
    updateRope();
});

function updateRope() {
    document.querySelector(".rope").style.marginLeft = `${ropePosition}px`;
}
